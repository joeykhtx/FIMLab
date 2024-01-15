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
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h2>Lessons Learned</h2>

- <b>The loop process of scanning and remediating to manage vulnerabilities</b>

<h2>Brush Up</h2>

- <b>Powershell Scripting </b>

<h2>Shortcuts Learned</h2>

- <b>-eq: Equal in Powershell</b>
- <b>.ToUpper: Reads input as Uppercase in Powershell</b> 


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
