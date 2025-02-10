<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create an Azure Virtual Machine Windows 10, 4 vCPUs / osTicket installation
- osTicket: Post-Installation Configuration
- osTicket: Tickets and Ticket Lifecycle 

<h2>Installation Steps</h2>

<p>
 1. <img src= "https://github.com/user-attachments/assets/8e9b2d8e-d27b-4024-a636-11d38e5999fa" height=80% width=80% alt="Disk Santization steps"/>
 <img src= "https://github.com/user-attachments/assets/00ed4d72-7bec-4780-b9f3-155a50657708" height=80% width=80% alt="Disk Santization steps"/> 
   <img src= "https://github.com/user-attachments/assets/d44e8570-cb50-481e-b9c0-c3a90f440bc4" height=80% width=80% alt="Disk Santization"/> 
   <img src= "https://github.com/user-attachments/assets/c886a675-b5d9-4ea7-912a-8b1291d72845" height=80% width=80% alt="Disk Santization"/>

 


</p>
<p>
 
- Name: osticket-vm
, Username: labuser
, Password: osTicketPassword1 
, Then created VM (virtual Machine).

 - Logged into the VM with Remote Desktop
 - VM (osticket-vm) downloaded the "osTicket-Installation-Files.zip" and unzipped it onto Remote Desktop (wil be using files in this folder to install some of the dependencies)   

</p>
<br />

<p>
2. <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Installed / Enabled IIS in Windows WITH CGI

- World Wide Web Services -> Application Development Features -> [X] CGI

- From the “osTicket-Installation-Files” folder, installed PHP Manager for IIS 


 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
