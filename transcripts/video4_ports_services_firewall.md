# Transcript: Ports, Services, Firewall Rules, and Scheduled Tasks (Video 4)

This video documents the 5.5 Prove assignment. I identified two active network ports and two running services, created inbound and outbound firewall rules for port 50000, and configured a daily scheduled task to install Windows updates automatically.

---

## 🎬 Summary

Using PowerShell and built-in Windows Server tools, I analyzed network activity and service status, configured custom firewall rules, and automated updates using Task Scheduler. This assignment highlights my ability to manage a secure and responsive server environment.

---

## 🛠️ Steps Performed

### 1. Identified Listening Ports
- Ran: `netstat -ano | findstr LISTENING`
- Chose:
  - **Port 3389**: Used for RDP (Remote Desktop Protocol)
  - **Port 5985**: Used for WinRM (Windows Remote Management)

### 2. Identified Running Services
- Ran: `Get-Service | Where-Object {$_.Status -eq "Running"}`
- Chose:
  - **TermService**: Supports RDP; listens on port 3389
  - **WinRM**: Enables remote command-line PowerShell access; uses port 5985

### 3. Created Firewall Rules for Port 50000 (TCP)
- Used **Windows Defender Firewall with Advanced Security**
- Created:
  - Inbound rule: “Custom Port 50000 Inbound”
  - Outbound rule: “Custom Port 50000 Outbound”
- Configured both to:
  - Allow TCP traffic
  - Be toggled (enabled/disabled) as needed without deletion

### 4. Scheduled Daily Windows Update
- Used **Task Scheduler**
- Created a task: `Daily Windows Update Check`
- Program: `powershell.exe`
- Arguments:
  ```powershell
  Install-WindowsUpdate -AcceptAll -AutoReboot
  
  Note: The task assumes the PSWindowsUpdate module is installed (which I confirmed)

## 🧠 Lessons Learned
- RDP and WinRM are core management ports that must be secured but available.
- PowerShell’s ability to filter services and automate tasks is incredibly powerful.
- Managing firewall rules manually gives better visibility than relying solely on Windows defaults.
- Scheduling updates via script helps ensure compliance and uptime.

## 🧰 Tools Used
- PowerShell
- Windows Defender Firewall
- Task Scheduler
- PSWindowsUpdate Module

## 🔗 [Watch the Video](https://youtu.be/ayMa6rTkbJ0)