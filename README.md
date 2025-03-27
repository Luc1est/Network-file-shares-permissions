# Network-file-shares-permissions



This tutorial outlines the Stepts to grant Access & permission in Active directory





<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Connect/log into DC-1 as your domain admin account-

- Connect/log into Client-1 as a normal user-

- On DC-1, on the C:\ drive, create 4 folders: “read-access”, “write-access”, “no-access”, “accounting”

<h2>Installation Steps</h2>


![image](https://github.com/user-attachments/assets/90ac0b92-776a-4907-9852-23558552afe9)


Open up the start menu, select windows administrative tools and then active directory users & computers.


![image](https://github.com/user-attachments/assets/46a05049-c5b9-452e-99c1-40f5f7a716bc)

Select ok.



![image](https://github.com/user-attachments/assets/22841afd-3678-4095-9fec-0e2978ada0be)

Select any user you'd like and remember their login information we will Return to this. within DC-1 we will create the following 4 Folders.“read-access”, “write-access”, “no-access”, “accounting”




![image](https://github.com/user-attachments/assets/a6dca3a3-d52c-4bc5-989a-488ad822392a)

 open up the start menu and click file explorer
 


![image](https://github.com/user-attachments/assets/21bf0125-a1ae-4a87-adb4-56831a67f7d6)

Click on this PC > Windows (c:) > Then Right click and select new folder



![image](https://github.com/user-attachments/assets/4312ef6f-e575-4a8f-a738-f90449a83483)
Create the following folders, Read-access, Write-Access, No-access, & Accounting

we will now enable the following permissions for the created folders: Set the following permissions (share the folder)
Folder: “read-access”, Group: “Domain Users”, Permission: “Read”
Folder: “write-access”,  Group: “Domain Users”, Permissions: “Read/Write”
Folder: “no-access”, Group: “Domain Admins”, “Permissions: “Read/Write”
(Skip accounting for now)






Select the read-access Folder >properties> sharing > share










