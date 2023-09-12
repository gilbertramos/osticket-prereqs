# osticket-prereqs<p align="center">
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

- Enable IIS
- PHP Manager
- Rewrite Module
- PHP 7.3.8 folder
- osTicket folder

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Begin by installing IIS.  Type in "run" in search bar of Windows, then enter "control".  Click on programs then Turn Windows features on or off.  Turn on folders "CGI", "Common HTTP Features".  Check and expand Internet Information Services.  Expand World Wide Web Services, then expand into Application Development Features.  Finally check the box next to CGI.  Go back to Common HTTP Features folder then expand it.  Check all boxes underneath Common HTTP Features.  This will install the IIS web server.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install PHP Manger Module and Rewirte Module.  Go to the C Drive, and a create a new folder named PHP.  Download the PHP zip folder and extract into the PHP folder on the C Drive. Then download and install the VC_redist.exe folder.  Next download the mysql-5.5.62-win32.msi folder, and create a username and password during the install.  Open the IIS as an Admin, this will open up the IIS Manager window.  Then doulbe click on PHP Manager.  Next click on "Register new PHP versions", browse to PHP on C drive then click on "php-cgi".  Click on the name of the server, then click on "Restart" on the upper right of the window. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the IIS as an Admin, this will open up the IIS Manager window.  Then doulbe click on PHP Manager.  Next click on "Register new PHP versions", browse to PHP on C drive then click on "php-cgi".  Click on the name of the server, then click on "Restart" on the upper right of the window. 
</p>
<br />
