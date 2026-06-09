# Active-Directory-Home-Lab
Active Directory Home Lab

## Project Overview

This project demonstrates the deployment and administration of a Windows Active Directory environment in a virtualized lab.

### Technologies Used

* Windows Server 2022
* Active Directory Domain Services (AD DS)
* DNS
* Group Policy
* Windows 11
* VirtualBox
* PowerShell

## Lab Architecture

### Virtual Machines

| Hostname | Role               | IP Address    |
| -------- | ------------------ | ------------- |
| DC01     | Domain Controller  | 192.168.10.10 |
| PC01     | Client Workstation | DHCP          |
| PC02     | Client Workstation | DHCP          |

## Objectives

* Install and configure Active Directory
* Create users and groups
* Join computers to the domain
* Configure Group Policy
* Deploy shared folders
* Troubleshoot authentication issues
* Practice PowerShell administration

## Active Directory Setup

### Domain Information

Domain Name:

homelab.local

### Organizational Units

* IT
* HR
* Sales
* Computers
* Groups

## User Management

Created users for multiple departments and tested:

* Password resets
* Account unlocks
* Account disablement
* Group membership management

## Group Policy Configuration

Configured policies for:

* Password complexity
* Account lockout
* Desktop wallpaper deployment
* Drive mapping
* USB restrictions

## File Shares

Created departmental shares:

* HR
* Sales
* IT

Configured:

* NTFS Permissions
* Share Permissions

## PowerShell Examples

Create User:

```powershell
New-ADUser
```

View Users:

```powershell
Get-ADUser -Filter *
```

Unlock User:

```powershell
Unlock-ADAccount
```

## Troubleshooting Scenarios

### Issue 1

User unable to log in.

Resolution:
Verified DNS settings and unlocked account.

### Issue 2

Mapped drive missing.

Resolution:
Verified Group Policy application and security group membership.

## Skills Demonstrated

* Active Directory Administration
* Windows Server
* DNS
* Group Policy
* User and Group Management
* PowerShell
* Troubleshooting
* Windows Networking

## Screenshots

Include screenshots showing:

1. Domain Controller
2. Active Directory Users and Computers
3. Group Policy Management
4. Shared Folder Permissions
5. Domain Joined Workstations
6. PowerShell Commands
