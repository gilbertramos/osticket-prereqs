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
- Heidi SQL

<h2>Installation Steps</h2>

<p>
<img width="821" alt="Screenshot 2023-09-14 101459" src="https://github.com/gilbertramos/osticket-prereqs/assets/140354494/8e961174-276a-4995-b879-fb4afe5f25d6">
</p>
<p>
Begin by installing IIS.  Type in "run" in search bar of Windows, then enter "control".  Click on programs then Turn Windows features on or off.  Turn on folders "CGI", "Common HTTP Features".  Check and expand Internet Information Services.  Expand World Wide Web Services, then expand into Application Development Features.  Finally check the box next to CGI.  Go back to Common HTTP Features folder then expand it.  Check all boxes underneath Common HTTP Features.  This will install the IIS web server.
</p>
<br />

<p>
<img width="874" alt="Screenshot 2023-09-14 105124" src="https://github.com/gilbertramos/osticket-prereqs/assets/140354494/11c8b700-1d90-4568-a0a1-7803e7b7a26c">
</p>
<p>
Download and install PHP Manger Module and Rewirte Module.  Go to the C Drive, and a create a new folder named PHP.  Download the PHP zip folder and extract into the PHP folder on the C Drive. Then download and install the VC_redist.exe folder.  Next download the mysql-5.5.62-win32.msi folder, and create a username and password during the install.  Open the IIS as an Admin, this will open up the IIS Manager window.  Then doulbe click on PHP Manager.  Next click on "Register new PHP versions", browse to PHP on C drive then click on "php-cgi".  Click on the name of the server, then click on "Restart" on the upper right of the window. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Download osTicket folder.  Extract and copy “upload” folder to c:\inetpub\wwwroot, then Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”.  Reload IIS again.  Go back to IIS, sites to Default to osTicket.  Double click the PHP Manager.  Then click "Enable or disable an extension" where you will click on "php_imap.dll", "php_intl.dll", "php_opcache.dll", and refresh the osticket website to see the changes.  Now rename ost-config.php From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to: C:\inetpub\wwwroot\osTicket\include\ost-config.php.  To assign premissions right click ost-config.php, goto properities, click on security, click on advanded, click on disable inheritance, finally click on remove all permissions.  Now click on the Add button, click on "Select principal", type in "Everyone" in the box then click "OK" then click "Full Control". Goto osTicket website, setup Help desk name, default email.  Download Heidi SQL, open file and install.  Open Heidi then click on "New", enter same user name and password from osTicket website, now click "Open".  Right click and hit "Create new" then select "Database".  Type in "osTicket" in the name box, click "Ok".  On the osTicket website fill out the fields under Database settings then click "Install Now". Delete C:\inetpub\wwwroot\osTicket\setup.  Goto C:\inetpub\wwwroot\osTicket\include\ost-config.php then set permissions to "Read" only.
</p>
<br />
