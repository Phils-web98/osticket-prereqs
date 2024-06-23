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
Use this link for reference and downloads
https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/1b313a9b-c06c-4a94-bf01-455c83246ba5)


- Enable IIS (Internet Information Services) in Windows with CGI and Common HTTP Features
 
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/38b6786d-01e4-488e-9f30-8b52076d725d)

  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/9bf2532d-4024-4055-b3f6-de146c56aa20)

- Instal PHP Manager for IIS (PHPManagerFORIIS_V1.5.0.msi)
  
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/aaf9f4be-16a3-4724-b8d6-fc6fe396b8f9)

- Install the Rewrite Module (rewrite_amd64_en-US.msi)

  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/73a384b5-84ef-4a30-a97e-3d7a5a543efd)

  
- Create a directory called C:\PHP on the local hard drive

   ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/7ba14ea6-af15-4b3a-92ae-e21b4c177db2)

- Download PHP 7.3.8 and Unzip files into C:\PHP

  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/0cfcc689-c902-4a75-ae6c-d5a47eea6534)

- Download VC redist.x86.exe

  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/5a86e865-5ba9-426d-959f-27b1d88e2ec6)

  
- Download MySQL 5.5.62 (mysql-5.5.62-win32.msi)
  1) Click Typical Setup --> launch configuration wizard --> Standard Configuration
  2) Create a password

   ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/711804e2-eb04-4c55-bf50-cdcded66e092)

   
- Configurations
  1) Register PHP from IIS as an adminstrator
   ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/645b3673-abe9-474c-84fe-4f9099172681)
  2) Restart the IIS server
     
- Download osTicket from installation Files
  1)Copy "upload" folder to c:\inetpub\wwwroot and Rename it to 'osTicket"
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/4fa1c015-5027-4c30-9577-67e7c06e329a)
  2) Rename it to 'osTicket"
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/61c8a07c-5d7a-4a90-8a01-ff394613bb87)
  3)Open IIS as admin, Click Sites then Defaut Website then osTicket then "Browse *.80"
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/2ef25c6a-11cf-43d7-abf5-c38d74aca37c)
  4) A webpage displaying osTicket should open
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/d0effce4-b4b6-4650-8de6-c3327f2d331f)
  Enable the remaining configurations
  5)Double-click PHP Manager on IIS, then "Enable or disable extension", enable "php_imap, php_intln, and php_opcache"
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/546b490b-5653-41f9-b164-79fa073cb495)
  6)Rename ost-sampleconfig in osTicket Folder to "ost-config.php"
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/08a9796f-1a3e-4a59-bf8d-2681ae2ed1a0)
  7)Disable inheritance and assign permission to all users to interact with ost-config file
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/0a84354a-d574-4980-a785-23f293802770)
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/04e45c63-9b7e-4da4-b837-1616f5dcec46)
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/dd495088-65fa-43ea-9725-5d34098d98b2)

  8) Install HeidiSQL
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/205e0249-4d36-4a18-9f5d-311b398ee5af)
  Create new connection (username is root and password is the one used in the SQL set up)
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/866a53f5-7904-4701-95f1-7fcf1c64dc7c)
  Create new database in Heidi, right-click "Unamed" then "new" then "database"
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/5a996b65-25af-4869-b9df-3022b141e5bf)


   
  9)osTicket Set-Up
  Click continue on the web browser, Fill up the necessary information
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/c021953a-8963-46b9-bfb3-3e1e16c56444)
  Use "osticket" as MySQL Database name from Heidi
  Use SQL username(root) and the password used for SQL
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/f72b73e3-b061-4924-aaba-2cb30755f7da)
  Click "Install"
  ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/c733279c-8ede-4bb5-a0fb-13927ed12622)

  10) Delete the setup folder C:\inetpub\wwwroot\osTicket\setup
      Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php
      ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/7b9c3b7c-0839-454d-b884-da135d6bf16a)
      
  11) Links
     For Admin: http://localhost/osTicket/scp/login.php
     ![image](https://github.com/Phils-web98/osticket-prereqs/assets/172346798/1fc3f271-a9b3-4749-bd94-65b6b87c0260)

     For End users: osTicket URL: http://localhost/osTicket/ 



  
 





  



  







<br />
