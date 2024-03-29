<h1>FIM (File Integrity Monitor) Lab</h1>


<h2>Description</h2>
With this lab we gain a better understanding of what integrity means in Cybersecurity through a live example of file integrity monitoring via a live demo. We will go through coding and build a File Integrity Monitor. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p>
In Powershell ISE, create a script that asks "What would you like to do?": <br/>
- Here we have the question and two answers</b> 
- Save and test script with Read-Host. Read-Host allowed us to read inputs in from the command line</b> 
<img src="https://i.imgur.com/TuUqRo5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create the two answers:  <br/>
This snip shows the two options (A and B) with the a test of input output at the shell level. <br/>
<img src="https://i.imgur.com/qNa1AR0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Make a new function that calculates the hash file: <br/>
Line 16 tests the funtion demonstrating an output showing the hash of the file.
<img src="https://i.imgur.com/zX32HrY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Write out the rule for Option A:  <br/>
This option collects all files in target folder and calculates the hash for them. It then stores the information output into the "baseline.txt file.  <br/>
<img src="https://i.imgur.com/PthvisR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Here we added a function that runs prior to the option of collecting a new baseline:<br/>
This funtion will get rid of the baseline.txt file in preparations to an updated baseline.txt file.
<img src="https://i.imgur.com/cBrJMfT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create our dictionary. Load all files from baseline.txt and store in our dictionary:  <br/>
The dictionary will store all the updated keys and values. In our case the keys were the file paths and the values were the hashes that corresponds to the files. In this example, we were able to test it by running the selection of line 51 ($fileHashDictionary.Keys or $fileHashDictionary.Values) and viewing the output in the console.
<img src="https://i.imgur.com/vMRG7lr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Here we added an infine loop that sleeps and checks every second to see if the files have changed by using a while loop: 
<br/>
The goal was to create a notification by printing something to the screen if any values was to change.
<img src="https://i.imgur.com/F38jlET.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
We then create a loop through each target file. This will then calculate the hash and compare the file|hash to what the baseline is then notify the hash is changed:<br/>
<img src="https://i.imgur.com/Cb8oGKB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a functions that checks if any of the files have been deleted. This would test the paths of the keys in the baseline. If any of those come back false then that would trigger an alert.
<img src="https://i.imgur.com/F38jlET.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

<h2>Lessons Learned</h2>

- <b>Dictionary - Data structure in language. Holds the key (file path) and value (corresponding hash) </b>

<h2>Brush Up</h2>

- <b>Powershell Scripting </b>

<h2>Shortcuts Learned</h2>

- <b>-eq: Equal in Powershell</b>
- <b>.ToUpper: Reads input as Uppercase in Powershell</b>
- <b>Get-Command *Hash*: Shows the funtion and command for the Get command</b>
- <b>.split(""): Splits command by the character inbetween the quotation marks. </b>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
