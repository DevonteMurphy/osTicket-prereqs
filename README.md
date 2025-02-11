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

</p>
<p>

(1. Create an Azure Virtual Machine Windows 10, 4 vCPUs / osTicket installation.
- Name: osticket-vm
, Username: labuser
, Password: osTicketPassword1 
, Then created VM (virtual Machine).
  <img src= "https://github.com/user-attachments/assets/8e9b2d8e-d27b-4024-a636-11d38e5999fa" height=80% width=80% alt="Disk Santization steps"/>
- Logged into the VM with Remote Desktop
  <img src= "https://github.com/user-attachments/assets/00ed4d72-7bec-4780-b9f3-155a50657708" height=80% width=80% alt="Disk Santization steps"/>
 
 - VM (osticket-vm) downloaded the "osTicket-Installation-Files.zip" and unzipped it onto Remote Desktop (will be using files in this folder to install some of the dependencies)   
   <img src= "https://github.com/user-attachments/assets/d44e8570-cb50-481e-b9c0-c3a90f440bc4" height=80% width=80% alt="Disk Santization steps"/>
   <img src= "https://github.com/user-attachments/assets/c886a675-b5d9-4ea7-912a-8b1291d72845" height=80% width=80% alt="Disk Santization steps"/>  
</p>
<br />
(2. osTicket: Post-Installation Configuration 
<p>

- Installed / Enabled IIS (internet information services) in Windows with CGI
  <img src="https://github.com/user-attachments/assets/8ed1d3d9-d9ac-4de5-ae0c-a32dd07f8af5" height="80%" width="80%" alt="Disk Sanitization steps"/>
  <img src="https://github.com/user-attachments/assets/a1dfa1a6-d2e7-4c66-8204-e3d4061b0921" height=80% width=80% alt="Disk Santization steps"/> 

- World Wide Web Services -> Application Development Features -> [X] CGI
  <img src="https://github.com/user-attachments/assets/fc0531e0-a0d6-4826-ba5c-74a5ee799aa9" height=20% width=55% alt="Disk santization steps"/>
  <img src="https://github.com/user-attachments/assets/d9df9bf0-36de-4271-bf7f-11ebe7d3c25e" height=20% width=55% alt="Disk Santization"/>

- From the “osTicket-Installation-Files” folder, installed PHP Manager for IIS 
 <img src="https://github.com/user-attachments/assets/7164bc7a-522d-4197-b3f3-c6cc5b260ba9"
height=50% width=50% alt="Disk santization"/>
  <img src="https://github.com/user-attachments/assets/080e403a-18d8-448a-8911-2496ba8c16e9" height=20% width=55% alt="Disk Santization"/> 

- From the “osTicket-Installation-Files” folder installed Rewrite Module (rewrite_amd64_en-US.msi) 
<img src="https://github.com/user-attachments/assets/4822fbe2-a0fe-43b1-bd75-6b3f7b141fff"  height=45% width=30% alt="Disk santization"/>
<img src="https://github.com/user-attachments/assets/3ac1446f-963c-42ae-88e1-d744760b74aa" height=65% width=30% alt="Disk santization"/>

- Created a directory C:\PHP
<img src="https://github.com/user-attachments/assets/84524a61-5216-426a-b733-663fdc1cdb12" height=35% width=45% alt="Disk Santization"/> 

- From the “osTicket-Installation-Files” , unzipped PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into “C:\PHP” folder
<img src="https://github.com/user-attachments/assets/42ce79da-26a4-457e-8f29-41752fbc86c0" height=35% width=45% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/ff18ae0b-7e91-48c1-b717-102c81f39d91" height=35% width=45% alt="Disk Santization"/>


- From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.
<img src="https://github.com/user-attachments/assets/79487ed8-02a4-4208-a48a-2f05f5562618" height=25% width=50% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/553a2512-4246-4ea5-8c4c-94db519b3451" height=25% width=50% alt="Disk Santization"/>

- From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi
<img src="https://github.com/user-attachments/assets/84c1a6d3-c3ae-4918-8fe5-af4a4dd965aa" height=25% width=50% alt="Disk santization"/>
<img srch="https://github.com/user-attachments/assets/8f04672d-7e7d-46eb-ab56-3315bd44c2b3" height=20% width=50% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/986c212a-eedc-42e1-87bd-740fd1040aa4" height=25% width=50% alt="Disk Santization"/>

- Open IIS as an Admin
<img src="https://github.com/user-attachments/assets/9d830895-24bf-4dfa-a2b6-b326c9ae2e31" height=40% width=40% alt="Disk santization"/>
<img src="https://github.com/user-attachments/assets/6d63b5f7-09a5-4ef1-9fa1-3293ceab3e2f" height=40% width=40% alt="Disk Santization"/>

- Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
<img src="https://github.com/user-attachments/assets/9b7ad435-e32e-4372-a05a-da67ce3c5c4d" height=40% width=40% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/09de6ac9-696c-49de-b461-c0b549c28eb7" height=35% width=40% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/e493782c-c4e7-4729-ab6a-4cf94e8e6b7f" height=80% width=40% alt="disk Santization"/>
<img src="https://github.com/user-attachments/assets/1d009b88-5277-4faa-91c6-d888463e5bcf" height=35% width=40% alt="Disk Santization"/>

- Installed osTicket v1.15.8
From the “osTicket-Installation-Files” folder, unzipped “osTicket-v1.15.8.zip” and copied “upload” folder into “c:\inetpub\wwwroot”
Within “c:\inetpub\wwwroot”, Renamed “upload” to “osTicket”
 <img src="https://github.com/user-attachments/assets/722934c6-39ff-441a-b01a-e3431826236d" height=50% width=25% alt="disk Santization"/>
 <img src="https://github.com/user-attachments/assets/af1a52e8-2393-4672-baee-bb4f2c814d08" height=50% Width=25% alt="Disk Santization"/>
 <img src="https://github.com/user-attachments/assets/12523f74-46fb-49d5-a8b4-a47f70281016" height=50% Width=25% alt="Disk Santization"/>
 <img src="https://github.com/user-attachments/assets/d7884f7e-8146-4256-9991-4269b679ecaf" height=50% width=25% alt="disk santization"/>
 <img src="https://github.com/user-attachments/assets/202ca6af-ee77-4222-ae1a-616446325c02" height=50% width=25% alt="Disk Santization"/>
 <img src="https://github.com/user-attachments/assets/3b97e85e-0784-4ef0-98ba-1dccb2ea4d0f" height=50% Width=25% alt="Disk Santization"/>
 <img src="https://github.com/user-attachments/assets/f49ea3f4-a598-4494-bad1-02beedfb2b27" height=50% width=25% alt="disk Santization"/>
 <img src="https://github.com/user-attachments/assets/deb8a277-bdd8-43ab-a5b2-dae1c913f058" height=50% width=25% alt="Disk Santization"/>


- Reload IIS (Open IIS, Stop and Start the server)
![image](https://github.com/user-attachments/assets/92736f70-91e9-42ed-a858-7010bb37c37c)
![image](https://github.com/user-attachments/assets/348a63e1-6273-4851-9822-81a0ab895356)

- Go to sites -> Default -> osTicket
 On the right, click “Browse *:80”
![image](https://github.com/user-attachments/assets/fae582e1-7062-48c3-9c36-3be859329438)
![image](https://github.com/user-attachments/assets/3adf4e6f-7082-427a-b3d8-b166da0e4e0f)

- Went back to IIS, sites -> Default -> osTicket
 Double-clicked PHP Manager


Some extensions are not enabled
- Click “Enable or disable an extension”
 Enable: php_imap.dll
 Enable: php_intl.dll
 Enable: php_opcache.dll
 Refresh the osTicket site in your browser, observe the changes

- Rename: ost-config.php
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

- Assign Permissions: ost-config.php
Disable inheritance -> Remove All
New Permissions -> Everyone -> All

- Continue Setting up osTicket in the browser (click Continue)
Name Helpdesk
Default email (receives email from customers)

- From the “osTicket-Installation-Files” folder, install HeidiSQL.
Open Heidi SQL
Create a new session, root/root
Connect to the session
Create a database called “osTicket”

- Continue Setting up osTicket in the browser
MySQL Database: osTicket
MySQL Username: root
MySQL Password: root
Click “Install Now!”


</p>
<br />
(3. osTicket: Tickets and Ticket Lifecycle 
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


</p>
<br />
