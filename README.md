<h1>SIEM/SOC Honeypot Lab Setup</h1>

 

<h2>Description</h2>
In this hands-on project, I built and deployed a personal Security Operations Center (SOC) by setting up a SIEM system using Microsoft Sentinel. The system is designed to monitor security events from a Windows Virtual Machine on Azure, with a focus on detecting unauthorized access attempts through RDP.
<br />


<h2>Utilities Used</h2>

- <b>Microsoft Azure</b> 
- <b>Microsoft Sentinel</b>
- <b>RDP</b>
- <b>Windows VM</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (21H2)

<h2> Key Skills & Technologies</h2>

- <b>Azure: Utilized Azure Free Tier to create and manage a Windows Virtual Machine (VM) and configure cloud-based security operations.</b>
- <b>Threat Monitoring: Configured alerts and monitoring for RDP (Remote Desktop Protocol) activity to detect unauthorized access attempts.</b>
- <b>Incident Response: Set up custom security alerts to automatically notify upon successful unauthorized login attempts, helping to simulate real-world cyberattack scenarios.</b>
- <b>Windows Security: Gained experience with event log collection, analysis, and management from a Windows VM using Azure Monitor Agent.</b>
- <b>Automation: Automated incident creation and alerting based on event detection, optimizing security monitoring workflows.</b>
- <b>Threat Intelligence: Integrated threat intelligence feeds to simulate and monitor indicators of compromise (IOCs) in a controlled environment.</b>


<h2>Lab walk-through:</h2>

<p align="center">
 Create an Azure Virtual Machine (VM): <br/>
<ul>
  <li>Go to <strong>Azure Portal</strong> and search for <strong>Virtual Machines</strong></li>
  <li>Click <strong>Create > Virtual Machine</strong></li>
  <li>Select <strong>Windows Pro</strong> as the OS</li>
  <li>Configure the following:
    <ul>
      <li><strong>Resource Group:</strong> Create a new one (e.g., <em>Mad Hat Group</em>)</li>
      <li><strong>Virtual Machine Name:</strong> (e.g., <em>MadHat-VM</em>)</li>
      <li><strong>Region:</strong> Select the preferred Azure region</li>
      <li><strong>Administrator Username:</strong> e.g., <em>madhathimself</em></li>
      <li><strong>Password:</strong> Secure password of your choice</li>
    </ul>
  </li>
  <li><strong>Allow RDP (Port 3389) Access</strong></li>
  <li>Click <strong>Review and Create</strong></li>
  <li>Wait for the VM to be deployed</li>
</ul>



<img src="Screenshot1.png" alt="Azure Virtual Machine Setup" width="800">

<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
  
