<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Traffic Inspection Among Azure Virtual Machines</h1>
In this tutorial, we will examine different network traffic patterns to and from Azure Virtual Machines using Wireshark. Additionally, we will conduct experiments involving Network Security Groups (NSGs). <br />




<h2>Utlized Environments and Technologies</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1- Downloaded Wireshark
- Step 2- Use Powershell
- Step 3- Creating a NSG rule
- Step 4- Request timed out
- Step 5- SSH Protocol
- Step 6- SSH Traffic
- Step 7- DNS Protocol
<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/d0HTJ2Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I installed an application called Wireshark. Wireshark is a protocol analyzer that enables you to monitor the traffic being generated and passing through a network in real-time.
</p>
<br />

<p>
<img src="https://i.imgur.com/G4Fi5k8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here, I utilized PowerShell to ping the private IP address of my second virtual machine, creating ICMP traffic to observe within Wireshark.
</p>
<br />
  
  <p>
<img src="https://i.imgur.com/mtkGa1j.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The continuous ping has now reached a timeout due to the rule I created. It has transformed from a request-reply pattern to a situation where only requests are sent without receiving any replies.
</p>
<br />

<p>
<img src="https://i.imgur.com/NfsaXQQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step, I will initiate an SSH (Secure Shell) connection to my second virtual machine from my first virtual machine using PowerShell.
</p>
<br />

<p>
<img src="https://i.imgur.com/3LfHa4s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here, I generated some traffic to examine for SSH activity.
</p>
<br />

<p>
<img src="https://i.imgur.com/d4hehWO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here, I am essentially making a DNS (Domain Name System) inquiry to determine Google's IP address.
</p>
<br />
