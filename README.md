<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


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

- Create file shares with various permissions
- Access file shares as normal user
- Create Security Group, and assign permissions 
  

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/MWaXUPx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are tasked with establishing file shares featuring tailored permissions to ensure access control aligns with individual user requirements. Stringent permissions will be enforced, denying access to unauthorized individuals and safeguarding the integrity of the content.
</p>
<br />

<p>
<img src="https://i.imgur.com/PULY2nW.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Each user will authenticate their credentials upon login to access files within designated directories. Authorized users will possess privileges to create new folders, peruse specified documents, and generate new text documents within the system.
</p>
<br />

<p>
<img src="https://i.imgur.com/6ZlwTj5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will establish a security group and meticulously assign permissions tailored to individual user roles and responsibilities. Subsequently, we will conduct comprehensive access testing with diverse user profiles to validate the efficacy of the permissions structure. Access privileges to specific files will be dynamically determined based on users' respective positions within the designated security group.
</p>
<br />
