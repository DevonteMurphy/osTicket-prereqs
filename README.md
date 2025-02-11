<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This Lab outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Created an Azure Virtual Machine Windows 10, 4 vCPUs / osTicket installation
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
<img src="https://github.com/user-attachments/assets/ff18ae0b-7e91-48c1-b717-102c81f39d91" height=35% width=40% alt="Disk Santization"/>


- From the “osTicket-Installation-Files” folder, installed VC_redist.x86.exe.
<img src="https://github.com/user-attachments/assets/79487ed8-02a4-4208-a48a-2f05f5562618" height=25% width=45% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/553a2512-4246-4ea5-8c4c-94db519b3451" height=25% width=45% alt="Disk Santization"/>

- From the “osTicket-Installation-Files” folder, installed MySQL 5.5.62 (mysql-5.5.62-win32.msi
<img src="https://github.com/user-attachments/assets/84c1a6d3-c3ae-4918-8fe5-af4a4dd965aa" height=25% width=50% alt="Disk santization"/>
<img srch="https://github.com/user-attachments/assets/8f04672d-7e7d-46eb-ab56-3315bd44c2b3" height=25% width=50% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/986c212a-eedc-42e1-87bd-740fd1040aa4" height=25% width=45% alt="Disk Santization"/>


- Opened IIS as an Admin
<img src="https://github.com/user-attachments/assets/9d830895-24bf-4dfa-a2b6-b326c9ae2e31" height=40% width=40% alt="Disk santization"/>

<img src="https://github.com/user-attachments/assets/6d63b5f7-09a5-4ef1-9fa1-3293ceab3e2f" height=40% width=40% alt="Disk Santization"/>

- Registered PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
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
<img src="https://github.com/user-attachments/assets/92736f70-91e9-42ed-a858-7010bb37c37c" height=35% width=45% alt="Disk Snatization"/>
<img src="https://github.com/user-attachments/assets/348a63e1-6273-4851-9822-81a0ab895356" height=35% width=45% alt="Disk Santization"/>

- Went to sites -> Default -> osTicket
 On the right, click “Browse *:80”
<img src="https://github.com/user-attachments/assets/fae582e1-7062-48c3-9c36-3be859329438" height=35% width=50% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/d96d596c-7b40-4950-aa1e-c36eede0e09e" height=35% width=45% alt="disk Santiztion"/>

- Went back to IIS, sites -> Default -> osTicket
 Double-clicked PHP Manager
<img src="https://github.com/user-attachments/assets/53c62c05-41f5-482a-85e2-893b0ad17f2e" height=35% width=45% alt="Disk Santization"/>

Some extensions were not enabled
- Went to “Enable or disable an extension”
 Enabled: php_imap.dll,
 Enabled: php_intl.dll,
 Enabled: php_opcache.dll, and
 Refreshed the osTicket site in browser
<img src="https://github.com/user-attachments/assets/007b531a-872f-4031-9e94-7544d4e12000" height=35% width=45% alt="Dsik Santization"/>
<img src="https://github.com/user-attachments/assets/782a253d-2fb4-4c40-9130-8d648307add6" height=35% width=45% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/d633d391-08f0-410d-bab3-8cd60a8ab42e" height=35% width=45% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/e5105fcb-d75c-4317-8e25-2dea1dd4346f" height=35% width=45% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/8b1b6190-44c5-4274-84bb-74fe0a471104" height=35% width=45% alt="Disk santization"/>
<img src="https://github.com/user-attachments/assets/e5415f69-fdf7-42f3-87c2-d25433abc08e" height=35% Width=45% alt="Disk Santization"/>


- Renamed: ost-config.php
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
<img src="https://github.com/user-attachments/assets/35161795-b5a2-4599-8c8b-ecdb4dd0be02" height=35% width=45% alt="Disk Santization"/>

- Assigned Permissions: ost-config.php
Disable inheritance -> Remove All
New Permissions -> Everyone -> All
<img src="https://github.com/user-attachments/assets/1a528386-aa2d-4f1d-9c74-c180506bccdd" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/c1cc49ca-18ee-403e-95d1-0bda72a71c7f" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/a08841bd-ee4d-4db3-bcb5-88465b94932a" height=35% width=35% alt="Disk santization"/>
<img src="https://github.com/user-attachments/assets/8254013a-cdee-450c-8af3-6a2438aa36e0" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/752284c6-58c0-4e38-a036-c3afded1fe00" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/c1d841c7-0367-4236-8aee-b1a150a13acd" height=35% width=35% alt="Disk Santiztion"/>

- From the “osTicket-Installation-Files” folder, installed HeidiSQL.
Open Heidi SQL
Created a new session, root/root
Connect to the session
Created a database called “osTicket”
<img src="https://github.com/user-attachments/assets/906cd25e-f1b3-45bd-9e0f-a34ff32a02c2" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/6cac1f60-43da-42ff-81f1-425d9542de9e" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/30f17234-1cd4-433c-a6d4-193824dc69f8" height=35% width=35% alt="Disk Santiztion"/>
<img src="https://github.com/user-attachments/assets/d14f9f1a-9907-4e48-90b5-1b81fc2d1d0c" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/fe094f8a-2d73-41ef-b66e-6e20718fb6e2" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/11524241-702b-4c14-af4e-fa7cca410101" height=35% width=35% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/1243b469-0826-459a-8fde-34464630a012" height=35% width=35% alt="Disk Santization"/>

- Setting up osTicket in the browser
MySQL Database: osTicket
MySQL Username: root
MySQL Password: root
<img src="https://github.com/user-attachments/assets/afb47af4-f7c1-4a0f-94e3-d5bd80f9e8a0" height=45% width=45% alt="Disk Santization"/>
<img src="https://github.com/user-attachments/assets/df23046d-fff6-424f-8329-59a25c3088c1" height=45% width=45% alt="Disk Santization"/>



</p>
<br />
(3. osTicket: Tickets and Ticket Lifecycle 
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


</p>
<br />
