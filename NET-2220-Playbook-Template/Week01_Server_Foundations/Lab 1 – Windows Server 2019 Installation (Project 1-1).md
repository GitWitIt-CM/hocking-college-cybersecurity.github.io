## Lab 1 – Windows Server 2019 Installation (Project 1-1)
**Student:** Cameron McKenzie  
**GitHub:** GitWitIt  
**Date Submitted:** 2025-11-03  

---

### **Task / Purpose**
Install Windows Server 2019 Datacenter (Desktop Experience) in a virtual environment, configure the Administrator account, verify OS details using PowerShell commands, and document the setup process for foundational server administration skills.

---

### **Environment / Tools**
- Oracle VirtualBox  
- Windows Server 2019 Datacenter (Desktop Experience) ISO  
- Windows PowerShell  
- System Properties panel  

---

### **Steps Performed**
1. Created a new VirtualBox VM (4 GB RAM, 2 CPU cores, 50 GB virtual disk).  
2. Attached the Windows Server 2019 Datacenter ISO as the boot device.  
3. Booted from the ISO and selected:  
   - *Windows Server 2019 Datacenter (Desktop Experience)*  
4. Accepted license terms → selected **Custom Install**.  
5. Deleted all existing partitions until only unallocated space remained.  
6. Installed Windows Server 2019 to the unallocated drive.  
7. After reboot, set the Administrator password to **Secret555**.  
8. Logged in as **Administrator** and reached the desktop.  
9. Opened PowerShell and ran the required verification commands:  
   ```powershell
   systeminfo
