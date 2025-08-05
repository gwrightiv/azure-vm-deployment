# Transcript: Promoting Azure VM to Domain Controller (Video 2)

This video walks through the process of promoting a previously deployed Azure Windows Server 2025 VM to a Domain Controller using Active Directory Domain Services (AD DS). This was part of the iterative lab project in my IT 235 coursework.

---

## 🎬 Summary

Starting from a cleanly deployed Windows Server 2025 instance, I installed the AD DS role, promoted the VM to a Domain Controller, and configured the domain name `ensign.corp`. I verified successful promotion and domain login using both graphical and command-line tools.

---

## 🛠️ Steps Performed

1. Opened **Server Manager** → “Add Roles and Features”
2. Selected **Active Directory Domain Services (AD DS)**
3. After installation, used the **Promotion Wizard** to:
   - Create a **new forest**
   - Name the domain: `ensign.corp`
   - Set a secure **DSRM password** (stored in an encrypted password vault)
4. Restarted the server after promotion
5. Opened **Active Directory Users and Computers** to verify the domain was active
6. Logged in via **Remote Desktop** as a domain admin (`ensign\wright235`)
7. Verified domain login via:
   - `whoami` in Command Prompt (`ensign\wright235`)
   - Task Manager → Users tab

---

## 🧠 Lessons Learned

- The **promotion wizard** was intuitive and guided all necessary steps.
- It's critical to **secure the DSRM password** to avoid losing access to AD recovery tools.
- Using both **CLI and GUI** to verify domain login ensures troubleshooting flexibility.
- Restart behavior is automatic after promotion — plan for it during deployment windows.

---

## 🧩 Challenges Faced

- Small typo in the domain name during initial testing (I almost typed `ensign.core` instead of `ensign.corp`)
- Getting used to navigating between tools like AD DS, ADUC, and Server Manager

---

## 🧰 Tools Used

- Azure Portal (existing VM)
- Server Manager
- Active Directory Domain Services
- Active Directory Users and Computers
- Command Prompt
- Task Manager

---

## 🔗 [Watch the Video](https://youtu.be/K5TKPErCNv0)

