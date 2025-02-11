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
1.
<p>
  <img src= "https://github.com/user-attachments/assets/8e9b2d8e-d27b-4024-a636-11d38e5999fa" height=80% width=80% alt="Disk Santization steps"/>
 <img src= "https://github.com/user-attachments/assets/00ed4d72-7bec-4780-b9f3-155a50657708" height=80% width=80% alt="Disk Santization steps"/> 
   <img src= "https://github.com/user-attachments/assets/d44e8570-cb50-481e-b9c0-c3a90f440bc4" height=80% width=80% alt="Disk Santization steps"/> 
   <img src= "https://github.com/user-attachments/assets/c886a675-b5d9-4ea7-912a-8b1291d72845" height=80% width=80% alt="Disk Santization steps"/>

 


</p>
<p>
 
- Name: osticket-vm
, Username: labuser
, Password: osTicketPassword1 
, Then created VM (virtual Machine).

 - Logged into the VM with Remote Desktop
 - VM (osticket-vm) downloaded the "osTicket-Installation-Files.zip" and unzipped it onto Remote Desktop (will be using files in this folder to install some of the dependencies)   

</p>
<br />
2.
<p>
 <img src="https://github.com/user-attachments/assets/8ed1d3d9-d9ac-4de5-ae0c-a32dd07f8af5" height="80%" width="80%" alt="Disk Sanitization steps"/>
<img src="https://github.com/user-attachments/assets/a1dfa1a6-d2e7-4c66-8204-e3d4061b0921" height=80% width=80% alt="Disk Santization steps"/> 
<img src="https://github.com/user-attachments/assets/fc0531e0-a0d6-4826-ba5c-74a5ee799aa9" height=20% width=55% alt="Disk santization steps"/>
<img src="https://github.com/user-attachments/assets/d9df9bf0-36de-4271-bf7f-11ebe7d3c25e" height=20% width=55% alt="Disk Santization"/> 
 <img src="https://github.com/user-attachments/assets/7164bc7a-522d-4197-b3f3-c6cc5b260ba9"
height=50% width=50% alt="Disk santization"/>
 <img src="https://github.com/user-attachments/assets/080e403a-18d8-448a-8911-2496ba8c16e9" height=20% width=55% alt="Disk Santization"/> 


</p>
<p>

- Installed / Enabled IIS (internet information services) in Windows WITH CGI

- World Wide Web Services -> Application Development Features -> [X] CGI

- From the “osTicket-Installation-Files” folder, installed PHP Manager for IIS 


 
</p>
<br />
3.
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
