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




 - Download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.MSI)

   
  

 
 <img src="https://i.imgur.com/drMeNxR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

   - Download and install Rewrite Module (rewrite_amd64_ne-US.msi)
    

<img src="https://i.imgur.com/ghFGArp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

   
   - Create the directory C:\PHP

   - <img src="https://i.imgur.com/SaoWtXU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

    

   - Download and install PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.Z) and unzip contents into C:\PHP

    
  <img src="https://i.imgur.com/0YJvDlx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

   - Download and install VC_redist.x86.exe.

 <img src="https://i.imgur.com/NAvzsi9.png" height="80%" width="80%" alt="Disk Sanitization Steps">

  
  - Download MySQL 5.5.62 (mysql-5.5.62-win32.msi)
  
  -Typical Setup
 
  -Launch Configuration Wizard (after install)
 
  -Standard Configuration
  
  -Password1   
  
  
  <img src="https://i.imgur.com/65cayQV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/hs5ffYS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/axHPAHX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 - Open IIS as admin
 - Register PHP from within IIS
 - Reload IIS (Restart server)

<img src="https://i.imgur.com/OaamSHX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<img src="https://i.imgur.com/WI8wek9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 Step 4. Installing OsTicket

 - Download osTicket from installation files folder
 - Extract and copy "upload" folder to c:\inetpub\wwwroot
 - Within c:\inetpub\wwwroot, Rename "upload" to "osTicket


<img src="https://i.imgur.com/Gn2nJhC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZqVfKSg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DNnR9tP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 (Restart IIS server)

 
  - On right click "Browse *:80
  - In IIS go to site->defaults->osTicket
  - Double click PHP Manager
  - Click Enable or disable an extension 


<img src="https://i.imgur.com/7HeI477.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/oZxsB9n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JZ1ayEj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/cIVF8ST.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 (Refresh osticket site in your browser)

   - Rename: ost-config.php
    
     -From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
     
     -To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

     <img src="https://i.imgur.com/804gyKf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
     

 - Assign Permissions: ost-config.php
       
   -Disable inheritance-> Remove all
        
   -New Permissions-> Everyone-> All
    
<img src="https://i.imgur.com/exGYbg4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 -
<img src="https://i.imgur.com/ghFGArp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ghFGArp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ghFGArp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ghFGArp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ghFGArp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>






    




<img src="https://iimgur.com/NAvzsi9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



</p>
<br />
