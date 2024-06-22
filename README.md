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

  



  







<br />
