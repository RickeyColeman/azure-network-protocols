<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1: First I created my two VM's, one operating on Windows 10 OS and the other on Ubuntu OS. Next, I remote desktopped into the windows 10 VM. Within the VM I downloaded and installed Wireshark. 
- Step 2: From within the VM, I downloaded and installed Wireshark. After installed, I opened it and filtered for ICMP traffic only. 
- Step 3: Next, I retrieved the IP address of the Ubuntu VM and perpetually pinged it from the Windows 10 VM. Then I went back into the Azure portal and navigated to the Ubuntu VM's Network Security Group and disabled incoming ICMP traffic. I then went back into the Windows 10 VM and observed the pings failing in Wireshark. 
- Step 4:Lastly, I filtered for SSH traffic only and from within the Windows 10 VM I SSH'd into the Ubuntu VM via its private IP address. I then typed command such as, username, pwd, and etc into the linux SSH connection and observed the SSH traffic spam. After that I observed the traffics of DHCP, DNS, and RDP.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
