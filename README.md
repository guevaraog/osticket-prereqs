# osticket-prereqs
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

- Computer set to IIS
- PHP Manager for IIS
- IIS URL Rewrite Module 2 
- Microsoft C++ Redistributable
- MySQL
- OsTicket Installer
<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/pIHUgpP.png" height="40%" width="40%" alt="Files"/>
</p>
<p>
These are the files I used to make osTicket function correctly.
</p>
<br />

<p>
<img src="https://i.imgur.com/uaQCJhH.png" height="40%" width="40%" alt="Resource Group"/>
</p>
<p>
First setup a resource group for your virtual machine. 
</p>
<br />

<p>
<img src="https://i.imgur.com/YRFlQP0.png" height="50%" width="50%" alt="Virtual Machine"/>
</p>
<p>
Next you will setup a virtual machine using windows 10.
</p>
<br />

<p>
<img src="https://i.imgur.com/Mc8qJOq.png" height="20%" width="20%" alt="ISS CGI and HTTP"/>
</p>
<p>
Install / Enable IIS CGI and common HTTP Features

</p>
<br />

<p>
<img src="https://i.imgur.com/K2MbbHI.png" height="40%" width="40%" alt="ISS Windows"/>
</p>
<p>
You can tell if you put it in IIS correctly by typing 127.0.0.1 which will pull up this website if it's in ISS otherwise it won't come up.
</p>
<br />

<p>
<img src="https://i.imgur.com/94FYBYo.png" height="30%" width="30%" alt="PHP Manager for IIS"/>
</p>
<p>
Next you will download and install PHP Manager for IIS
</p>
<br />

<p>
<img src="https://i.imgur.com/0X0jW6a.png" height="30%" width="30%" alt="Rewrite Module"/>
</p>
<p>
Next you will download and install Rewrite Module.
</p>
<br />

<p>
<img src="https://i.imgur.com/7DlCCmu.png" height="40%" width="40%" alt="C:/PHP"/>
</p>
<p>
Next you will create a folder named PHP in C:/ drive. You will then dowload and unzip PHP inside of this folder and the files inside should look like the picture above.
</p>
<br />

<p>
<img src="https://i.imgur.com/0nAiEyy.png" height="40%" width="40%" alt="Visual C++"/>
</p>
<p>
Next you will download and install Visual C++.
</p>
<br />

<p>
<img src="https://i.imgur.com/SBtC7du.png" height="30%" width="30%" alt="SQL"/>
</p>
<p>
Next you will download and install SQL. 
</p>
<br />

<p>
<img src="https://i.imgur.com/9LmnIC9.png" height="40%" width="40%" alt="Register PHP"/>
</p>
<p>
Next you will open IIS as admin and register and restart server so changes are applied. 
</p>
<br />

<p>
<img src="https://i.imgur.com/61pjSFs.png" height="40%" width="40%" alt="wwwroot folder"/>
</p>
<p>
Download osTicket from the Installation Files Folder
Extract and copy “upload” folder to c:\inetpub\wwwroot and within c:\inetpub\wwwroot rename “upload” to “osTicket”
</p>
<br />

<p>
<img src="https://i.imgur.com/QZLg9vL.png" height="40%" width="40%" alt="osTicket installed!"/>
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server),
Go to sites -> Default -> osTicket
On the right, click “Browse *:80” and you will see osTicket pop up. 
<br />
Note that some extensions are not enabled
<br />
Go back to IIS, sites -> Default -> osTicket
<br />
Double-click PHP Manager
<br />
Click “Enable or disable an extension”
<br />
Enable: php_imap.dll
<br />
Enable: php_intl.dll
<br />
Enable: php_opcache.dll
<br />
Refresh the osTicket site in your browse, observe the changes.
</p>
<br />

<p>
<img src="https://i.imgur.com/QZLg9vL.png" height="40%" width="40%" alt="osTicket installed!"/>
</p>
<p>
Go to sites -> Default -> osTicket
On the right, click “Browse *:80” and you will see osTicket pop up. 
</p>
<br />

<p>
<img src="https://i.imgur.com/QZLg9vL.png" height="40%" width="40%" alt="osTicket installed!"/>
</p>
<p>
Go to sites -> Default -> osTicket
On the right, click “Browse *:80” and you will see osTicket pop up. 
</p>
<br />

