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
This snip shows the two options (A and B) with the a test of input output at the shell level.
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
Here we added a function that runs prior to the option of collecting a new baseline:  <br/>
<img src="https://i.imgur.com/cBrJMfT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Load all files from baseline.txt and store in our dictionary:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
