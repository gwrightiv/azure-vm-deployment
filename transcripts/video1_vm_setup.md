# Transcript: Azure VM Setup (Video 1)

This video documents the initial deployment of my Azure Windows Server 2025 VM for the IT 235 class.

---

## 🎬 Summary

I provisioned a Windows Server 2025 Datacenter Edition (Azure edition) VM in the East US 2 (Zone 2) region. I used Azure defaults where needed, and configured auto-shutdown to manage credit consumption. The VM was verified to meet course requirements (2023+), and RDP access was tested and confirmed.

---

## 🧾 Key Details

- **VM Name**: `wright235`
- **OS**: Windows Server 2025 Datacenter (Azure Edition)
- **Region**: East US 2 (Zone 2)
- **VM Size**: 2 vCPUs, 8 GB RAM
- **Hypervisor**: Azure-managed (Type 1 equivalent)
- **Previous experience**: Only with VirtualBox (Type 2 hypervisor)

---

## 🛠️ Steps Performed

1. **Created the VM** using the Azure wizard
2. **Downloaded and launched** the `.rdp` file
3. **Connected via Remote Desktop**
4. **Verified VM name and specs**
5. **Enabled auto-shutdown** in Azure at 10:00 PM EST
6. **Received shutdown notifications** via email

---

## 🧠 Lessons Learned

- This was my **first time provisioning a server in Azure**.
- I learned the importance of **setting zones properly**, as some were restricted.
- Auto-shutdown is **critical to avoid consuming all credits** — Azure estimated $165/month if left running.
- Managing costs is a **core part of cloud administration**, even in a lab setting.

---

## 🧩 Challenges Faced

- Choosing a valid zone (Zone 3 wasn’t allowed)
- Understanding how Azure billing ties directly into uptime and specs
- Learning Azure’s automation tools for shutdown scheduling

---

## 🔗 [Watch the Video](https://youtu.be/npShHMi-Ubo)

