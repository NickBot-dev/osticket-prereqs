<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Within the virtual machine, download the osTicket-Installation-Files.zip and unzip it onto the desktop. The folder should be called “osTicket-Installation-Files.”
 The files in this folder are used to install osTicket and some of the dependencies.

- Install / Enable Internet Information Services (IIS) in Windows, along with CGI
World Wide Web Services -> Application Development Features -> enable CGI

- Install the Web Server (PHP Manager) from within the “osTicket-Installation-Files” folder (PHPManagerForIIS_V1.5.0.msi). Followed by installing the Rewrite Module (rewrite_amd64_en-US.msi). Create a new folder on the C drive and rename it PHP. Extract all PHP files into to the new PHP folder on the C drive.
 

- From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi) and HeidiSQL to create the database. Rename to osTicket.  
Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Set credentals 

- Open IIS as an Admin... Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe). Reload IIS (Open IIS, Stop and Start the server)

- Install osTicket v1.15.8
From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”
Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”

<h2>Installation Steps</h2>

<p>

 ![sc](https://github.com/user-attachments/assets/7e265625-d5d8-4986-9df0-9c95b348119b)

</p>
<p>
From the start menu, open control panel and click on "uninstall or change a program". Next, click "turn Windows features on or off". Check Internet Information Services followed by expanding the folder to also check CGI. This is important to ensure that the web server is properly installed. 
</p>
<br />

<p>

 ![image](https://github.com/user-attachments/assets/bfd7ff86-3571-4065-8b2b-3dfb87dd681f)

</p>
<p>
 PHP Manager is a tool used for managing PHP installations on a Windows server, particularly with Internet Information Services (IIS). PHP Manager helps administrators manage multiple PHP versions and configure various PHP settings without manually editing configuration files or performing complex command-line operations. The Rewrite Module (rewrite_amd64_en-US.msi) is a dependency for installation followed by creating the new PHP folder on the C drive and extracting all PHP files into the new folder to unsure osTicket is properly configured. 

</p>
<br />

<p>

 ![image](https://github.com/user-attachments/assets/5aa0e194-5c93-4076-9c33-8a4a81a69b8e)

</p>
<p>
MySQL is an open-source relational database management system (RDBMS). It's used to store, retrieve, and manage data in structured formats using SQL (Structured Query Language).  
</p>
<br />


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
