## Lab 3 – Post-Installation Configuration & Verification  
**Student:** Cameron McKenzie  
**GitHub:** GitWitIt  
**Date Submitted:** 2025-11-14  

---

### **Task / Purpose**
Perform essential post-installation configurations on a Windows Server 2019 virtual machine.  
This includes hostname changes, firewall adjustments, time zone setup, network verification, and browser installation.  
All changes are documented with screenshots and PowerShell outputs.

---

### **Environment / Tools**
- Oracle VirtualBox  
- Windows Server 2019 Datacenter (Desktop Experience)  
- Server Manager  
- Windows PowerShell  
- Internet Explorer / Google Chrome  

---

### **Steps Performed**

1. Booted Windows Server 2019 and logged in as **Administrator (Secret555)**.  
2. Opened **Server Manager → Local Server** and reviewed system details.  
3. Updated date and time settings, including selecting the correct **Eastern Time** zone.  
4. Disabled **IE Enhanced Security Configuration** for Administrators.  
5. Opened Windows Firewall settings and turned firewall **Off** for Domain, Private, and Public profiles (lab environment).  
6. Collected network configuration details (IPv4, IPv6, DNS, gateway).  
7. Ran PowerShell commands for verification:
   - `ipconfig /all`
   - `Test-Connection 8.8.8.8 -Count 3`
8. Changed the computer name to **SERVER1** and restarted the VM.  
9. Verified activation state in Server Manager.  
10. Installed Google Chrome from Internet Explorer and confirmed external connectivity.  

---

### **Evidence / Screenshots**

#### Screenshot 1 – Local Server Properties Page
![Screenshot 179](./Screenshot%20(179).png)

#### Screenshot 2 – Date and Time / Time Zone Configuration
![Screenshot 180](./Screenshot%20(180).png)

#### Screenshot 3 – Windows Firewall Profiles Turned Off
![Screenshot 181](./Screenshot%20(181).png)

#### Screenshot 4 – Network Adapter Status & Details
![Screenshot 182](./Screenshot%20(182).png)

#### Screenshot 5 – PowerShell Output (ipconfig /all)
![Screenshot 183](./Screenshot%20(183).png)

#### Screenshot 6 – PowerShell Output (Test-Connection 8.8.8.8)
![Screenshot 184](./Screenshot%20(184).png)

#### Screenshot 7 – Renamed Server (SERVER1) – Post-Restart Verification
![Screenshot 185](./Screenshot%20(185).png)

#### Screenshot 8 – Google Chrome Installed and Connected to Internet
![Screenshot 186](./Screenshot%20(186).png)

---

### **Results**
All post-installation tasks were completed successfully.  
Time zone and firewall settings updated correctly.  
Hostname changed to SERVER1 and verified after reboot.  
Network settings were confirmed using PowerShell.  
Chrome installation verified external connectivity and browsing capability.

---

### **Reflection / Lessons Learned**
This lab demonstrated the importance of configuring a server immediately after installation.  
Time zone accuracy, firewall management, and hostname consistency all play a key role in server administration.  
Disabling the firewall in a lab environment is useful for testing, but in production systems, edge firewalls or hardware firewalls usually handle security.  
Network verification with tools like `ipconfig` and `Test-Connection` is essential for diagnosing connectivity.

---

### **Reproducibility Notes**
To recreate these results:
1. Install Windows Server 2019 and open **Server Manager → Local Server**.  
2. Adjust system time, time zone, and IE security options.  
3. Disable firewall profiles for lab use.  
4. Gather network details and verify connectivity via PowerShell.  
5. Rename the system and restart.  
6. Install Chrome via Internet Explorer and test browsing.

---



