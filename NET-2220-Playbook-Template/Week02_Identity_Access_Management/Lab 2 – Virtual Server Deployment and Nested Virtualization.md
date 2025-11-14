## Lab 2 – Virtual Server Deployment and Nested Virtualization  
**Student:** Cameron McKenzie  
**GitHub:** GitWitIt  
**Date Submitted:** 2025-11-14  

---

### **Task / Purpose**
Deploy a Windows Server 2019 Datacenter (Desktop Experience) virtual machine in VirtualBox, configure bridged networking for external connectivity, enable nested virtualization, verify system configuration using PowerShell commands, and document the results. Optional comparison with AWS for hybrid experience.

---

### **Environment / Tools**
- Oracle VirtualBox  
- Windows Server 2019 Datacenter ISO  
- VBoxManage (for enabling nested virtualization)  
- Windows PowerShell  
- Host system with VT-x / AMD-V support  

---

### **Steps Performed**

1. Opened VirtualBox and selected the existing Windows Server 2019 VM.  
2. Updated VM hardware configuration to match lab requirements:
   - RAM set to required amount  
   - 2 CPU cores  
   - Confirmed virtual disk size  
3. Opened **Settings → Network → Adapter 1** and switched to **Bridged Adapter** so the VM receives an IP from the host network.  
4. Ensured ISO was attached under **Storage**.  
5. Powered off the VM to enable nested virtualization.  
6. Ran the following command on the host (as Administrator) to activate nested virtualization:  
   `VBoxManage modifyvm "WindowsServer2019" --nested-hw-virt on`  
7. Started the VM and logged in as Administrator.  
8. Verified installation and virtualization support using PowerShell commands:  
   - `systeminfo`  
   - `systeminfo | find "Hyper-V Requirements"`  
   - `ipconfig /all`  
   - `ping 8.8.8.8`  
   - `Get-ComputerInfo | Select WindowsProductName, OsVersion, CsManufacturer, CsModel`  
9. Collected screenshots of networking, virtualization verification, and server desktop.  

---

### **Evidence / Screenshots**

#### Screenshot 1 – VirtualBox Network Settings (Bridged Adapter)
![Screenshot 172](./Screenshot(172).png)

#### Screenshot 2 – VM Settings (CPU, RAM, Storage)
![Screenshot 173](./Screenshot%20(173).png)

#### Screenshot 3 – Desktop After Login (Administrator)
![Screenshot 174](./Screenshot%20(174).png)

#### Screenshot 4 – PowerShell Output (systeminfo)
![Screenshot 175](./Screenshot%20(175).png)

#### Screenshot 5 – PowerShell Output (ipconfig /all & ping 8.8.8.8)
![Screenshot 176](./Screenshot%20(176).png)

#### Screenshot 6 – Hyper-V Requirements + Get-ComputerInfo Output
![Screenshot 178](./Screenshot%20(178).png)

---

### **Results**
The Windows Server 2019 Datacenter VM successfully booted using bridged networking, allowing it to obtain an IP address on the local network.  
Nested virtualization was successfully enabled using VBoxManage, and `systeminfo` confirmed the hypervisor and virtualization extensions.  
PowerShell outputs verified system configuration, network connectivity, and OS version information.

---

### **Reflection / Lessons Learned**
This lab demonstrated how VirtualBox handles bridged networking and virtual hardware configuration compared to default NAT mode. I also learned how nested virtualization works in VirtualBox, including how to enable it and verify it from inside the guest OS. Understanding Hyper-V Requirements and virtualization flags is important for future labs involving hypervisors, containers, and sandboxing technologies.

---

### **Reproducibility Notes**
To recreate this environment:
1. Create or use an existing Server 2019 VM in VirtualBox.  
2. Shut down the VM to modify hardware, networking, and virtualization settings.  
3. Enable nested virtualization via:  
   `VBoxManage modifyvm "WindowsServer2019" --nested-hw-virt on`  
4. Use Bridged Adapter for external connectivity.  
5. Boot the VM and run verification commands in PowerShell.  

---

### **Optional AWS Comparison (Not Completed)**
(If completed later, add AWS screenshots + comparison paragraph here.)


