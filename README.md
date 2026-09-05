# Windows Server & Active Directory Infrastructure Lab

## 📌 Project Overview
A practical hands-on lab demonstrating the setup and configuration of a Windows Server environment. It covers setting up Active Directory, managing users, sharing network files, and connecting a Windows 10 client machine.

## 🛠️ Lab Setup
- **Virtualization:** Oracle VirtualBox
- **Servers:** Windows Server (Domain Controller)
- **Clients:** Windows 10
- **Domain Name:** `HQ.corp`
  
  <img width="1329" height="746" alt="VirtualBox Setup" src="https://github.com/user-attachments/assets/0d6ea268-b91a-47fa-8044-4931cdd088d9" />


## ⚙️ What I Configured

### 1. Active Directory & Users
- Installed Active Directory Domain Services and created the `HQ.corp` domain.
- Created Organizational Units (OUs) to separate the **HR** and **IT** departments.
- Added users to Security Groups (`HR_Group`, `IT_Group`) to easily manage their permissions.

<img width="1196" height="692" alt="AD_Structure" src="https://github.com/user-attachments/assets/b7d28dca-fdb8-4dd6-bc73-82ca216cf491" />


### 2. Connecting Windows 10 to the Domain
- Configured the Windows 10 network settings to use the Windows Server as its DNS.
- Successfully joined the Windows 10 client to the `HQ.corp` domain.
- Logged in successfully from the client machine using a domain user account.

<img width="1008" height="761" alt="Windows 10 Domain Join" src="https://github.com/user-attachments/assets/720d6c74-3870-48f5-84b7-5c8a643a809c" />


### 3.  User Management
- Practiced common IT helpdesk tasks directly from Active Directory.
- Reset user passwords and disabled test accounts to understand basic administration controls.

<img width="958" height="594" alt="User_Management" src="https://github.com/user-attachments/assets/b2287197-4b27-4e90-a208-95de3fcc150c" />


### 4. File Sharing & Permissions
- Created network shared folders for the HR and IT departments.
- Configured **Share Permissions** and **NTFS Permissions** so that only members of the correct department group can access, read, or write their files.

<img width="1121" height="658" alt="NTFS_Permissions" src="https://github.com/user-attachments/assets/10e5f2ac-3319-4eaf-8dc4-06f5f80c2398" />


### 5. Roaming Profiles
- Set up Roaming Profiles so users can log into any PC on the network and have their personal files and desktop sync automatically.
- Configured the user profile path to point to a shared folder on the server (`\\Server\Profiles\%username%`).

<img width="952" height="621" alt="Roaming_Profile" src="https://github.com/user-attachments/assets/14da7304-cf93-4c29-b6a4-1e4020ebf512" />


### 6. Group Policy (GPO) Security
- Managed central security settings by configuring Group Policy Objects (GPOs).
- Enforced a stricter password policy, increasing the minimum password length requirement to 8 characters instead of the default 7.
- Secured user workstations by restricting access to the Control Panel, preventing unauthorized system changes by standard users.

<img width="1353" height="731" alt="Group Policy Configuration" src="https://github.com/user-attachments/assets/7986632b-5e8a-48c7-9641-8c47c6957752" />


## 🎯 Summary
This lab helped me apply my networking skills in a practical environment. I learned how to set up a basic domain, manage user accounts, and secure shared files using standard Windows Server tools.
