# Azure Windows Server Lab (Multi-Stage SysAdmin Project)

This repo documents a four-part iterative lab project I completed using Microsoft Azure and Windows Server 2025. It follows the full lifecycle of deploying, configuring, and securing a cloud-hosted domain controller — covering core sysadmin responsibilities including Active Directory setup, user/group management, firewall rules, and scheduled automation.

Completed as part of my IT System Administration coursework at Ensign College.

# Azure Windows Server Lab (Multi-Stage SysAdmin Project)

This repo documents a four-part iterative lab project I completed using Microsoft Azure and Windows Server 2025. It follows the full lifecycle of deploying, configuring, and securing a cloud-hosted domain controller — covering core sysadmin responsibilities including Active Directory setup, user/group management, firewall rules, and scheduled automation.

Completed as part of my IT System Administration coursework at Ensign College.

## 🧭 Project Progression

| Stage | Description |
|-------|-------------|
| ✅ 1 | **Azure VM Deployed** (Windows Server 2025, RDP enabled, auto-shutdown configured) |
| ✅ 2 | **Promoted to Domain Controller** (`ensign.corp` created, verified login as domain admin) |
| ✅ 3 | **Configured Active Directory** (Users + OUs, NTFS folder structure, permission mapping) |
| ✅ 4 | **Secured and Automated** (Firewall rules on port 50000, scheduled daily updates via Task Scheduler) |

## 🎥 Video Walkthroughs

Each stage includes a narrated video demo and a transcript.

1. [Azure VM Setup](transcripts/video1_vm_setup.md)
2. [Domain Controller Promotion](transcripts/video2_promote_to_dc.md)
3. [AD Users, Folders, and NTFS Permissions](transcripts/video3_users_ou_permissions.md)
4. [Ports, Services, Firewall & Updates](transcripts/video4_ports_services_firewall.md)

## 📸 Screenshots

Key setup and configuration visuals:

- [VM Overview (Azure Portal)](screenshots/azure-vm-overview.png)
- Server Properties (Windows Server 2025)
- Active Directory Domain Services Installed
- OU Structure in ADUC
- NTFS Permissions for Department Folders
- Custom Firewall Rule (Port 50000)
- Scheduled Task for Windows Updates

## 🧠 What I Learned

- How to provision a Windows Server in Azure using modern configurations
- How to promote a server to a domain controller using best practices
- The relationship between AD OUs, folder structure, and NTFS permissions
- How to secure a Windows server with inbound/outbound firewall rules
- PowerShell scripting and GUI tools for task scheduling and service control
- Importance of cost management with auto-shutdown in cloud environments

## 🛠️ Tools and Technologies

- Azure Portal
- Windows Server 2025 (Datacenter, Azure Edition)
- Active Directory Domain Services
- ADUC (Users and Computers)
- NTFS File System & Permissions
- PowerShell & PSWindowsUpdate Module
- Task Scheduler
- Windows Defender Firewall

