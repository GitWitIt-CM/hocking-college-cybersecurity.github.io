## Lab 1 – Windows Server 2019 Installation (Project 1-1)
**Student:** Cameron McKenzie  
**GitHub:** GitWitIt  
**Date Submitted:** 2025-11-14  

---

### Task / Purpose
Install Windows Server 2019 Datacenter (Desktop Experience) in a virtual environment, configure the Administrator account, verify OS details using PowerShell commands, and document the setup process for foundational server administration skills.

---

### Environment / Tools
- Oracle VirtualBox  
- Windows Server 2019 Datacenter (Desktop Experience) ISO  
- Windows PowerShell  
- System Properties panel  

---

### Steps Performed
1. Created a new VirtualBox VM with:
   - 4 GB RAM  
   - 2 CPU cores  
   - 50 GB virtual disk  
2. Attached the Windows Server 2019 Datacenter ISO as the boot device.  
3. Booted from the ISO and selected "Windows Server 2019 Datacenter (Desktop Experience)".  
4. Accepted the license terms and chose Custom Install.  
5. Deleted all existing partitions until only unallocated space remained.  
6. Installed Windows Server 2019 on the unallocated drive.  
7. After reboot, set the Administrator password to Secret555.  
8. Logged in to the server as Administrator.  
9. Opened PowerShell and ran the verification commands:
   - systeminfo
   - Get-ComputerInfo | Select WindowsProductName, OsVersion, CsManufacturer, CsModel
10. Opened System Properties to confirm OS edition and virtual hardware.

---

### Evidence / Screenshots
 

---

### Results
The Windows Server 2019 Datacenter VM installed successfully in VirtualBox.  
PowerShell verification confirmed correct OS version, product name, and VirtualBox hardware detection.  
System booted normally and responded correctly to administrative commands.

---

### Reflection / Lessons Learned
This lab helped me understand the full installation workflow of Windows Server 2019. I learned how to select the proper edition, perform a clean install, configure the Administrator account, and verify server details. Using systeminfo and Get-ComputerInfo helped reinforce how to validate server configuration after deployment.

---

### Reproducibility Notes
To recreate:
1. Create a VirtualBox VM (4 GB RAM, 2 cores, 50 GB disk).  
2. Boot from the Windows Server 2019 Datacenter ISO.  
3. Choose Custom Install, delete partitions, and install fresh.  
4. Set Administrator password to Secret555.  
5. Run the same PowerShell commands and collect screenshots.

