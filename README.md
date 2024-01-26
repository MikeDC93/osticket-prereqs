<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- PHP Manager for IIS
- Rewrite Module
- PHP 7.3.8
- Visual C++ Redistributable (VC_redist.x86.exe)
-  MySQL 5.5.62

<h2>Installation Steps</h2>

<p>
Step 1. Create a virtual machine in Azure

- Create a resource group
- Create a windows 10 virtual machine (VM)

   a. Name virtual machine VM-osticket

  b. For username use labuser (Can be anything)

   c. For password use osTicketPassword1 (Can be anything) 
<img src="https://i.imgur.com/4eyhbfM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2. Turn on / enable features in Windows

- Install / Enable IIS ( Internet Information Services) in Windows with CGI and Common HHTP Featrues.

  (Steps to enable, All steps in IIS)

   a. World Wide Services-> Application Development Features-> Mark CGI box
 
   b. World Wide Web Services-> Common HTTP Features-> Mark all boxs

   c. IIS-> Web Management-> IIS Management-> Mark IIS Management Console

  
</p>
<br />
a.
<img src="https://i.imgur.com/cWlAEnj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

b.

<img src="https://i.imgur.com/RXK1kSL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

c.

<img src="https://i.imgur.com/cWlAEnj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 3. Install prerequisites

(Prerequisites Files)

<img src="https://i.imgur.com/IlygbgL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>

</p>
<p>
- Download and instal PHP Manager for IIS (PHPManagerForIIS_V1.5.0.MSI)


   <img src="https://i.imgur.com/drMeNxR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

   - Download and install Rewrite Module (rewrite_amd64_ne-US.msi)

   - <img src="https://i.imgur.com/ghFGArp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
   - 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
