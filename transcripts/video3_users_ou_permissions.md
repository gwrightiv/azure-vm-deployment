# Transcript: Active Directory Users, OUs, and NTFS Permissions (Video 3)

This video documents the completion of the Users and Computers assignment (4.7 Prove) using Active Directory on a Windows Server 2025 domain controller.

---

## 🎬 Summary

I created Organizational Units (OUs) for different departments, added user accounts directly into their corresponding OUs, created a departmental folder structure on the C: drive, and assigned NTFS permissions to each user based on the assignment’s access control matrix.

---

## 🛠️ Steps Performed

### 1. Created Organizational Units (OUs)
In *Active Directory Users and Computers*, I created the following OUs:
- Employees
- HR
- IT
- Management
- Research
- Stakeholders
- Accounting
- Auditors

These were created under the domain `ensign.corp`.

### 2. Created 14 User Accounts
I added users directly into their proper OUs using the “New → User” option:
- HR: Sarah
- Research: Ted, Phil
- IT: Murtaugh
- Stakeholders: Spencer, Tim, Dean
- Management: Janine, Frank, Pearl
- Auditors: Sally, Bruce
- Accounting: Stephen, Guy

I set default passwords, enabled the accounts, and confirmed each user appeared in the correct OU.

### 3. Created Folder Structure
On the C: drive, I created:
    C:\PromisedLand
    ├── Accounting
    ├── Auditors
    ├── HR
    ├── IT
    ├── Management
    ├── Research
    └── Stakeholders


Each folder was matched to an OU for assignment of permissions.

### 4. Assigned NTFS Permissions
Using the *Properties → Security* tab on each folder, I assigned the following:

| Folder       | Users                       | Permissions     |
|--------------|-----------------------------|-----------------|
| Accounting   | Stephen, Guy                | Modify          |
| Auditors     | Sally, Bruce                | Full Control    |
| HR           | Sarah                       | Full Control    |
| IT           | Murtaugh                    | Full Control    |
| Management   | Janine, Frank, Pearl        | Read & Write    |
| Research     | Ted, Phil                   | Modify          |
| Stakeholders | Spencer, Tim, Dean          | Modify          |

I showed both GUI navigation and security tab configuration for each user.

---

## 🧠 Lessons Learned

- Creating users *directly in their OUs* saved time versus moving them after.
- NTFS permissions can be tricky — attention to detail is key.
- The difference between “Read/Write” and “Modify” required careful confirmation.
- Troubleshooting (e.g. accidentally adding the wrong user) is a normal part of sysadmin work, and knowing how to fix it matters.

---

## 🧰 Tools Used

- Active Directory Users and Computers (ADUC)
- File Explorer
- NTFS Security tab
- Windows Server 2025 (domain controller)

---

## 🔗 [Watch the Video](https://youtu.be/hFWW-Em5pkk)
