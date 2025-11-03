# Playbook Entry — Week 01: Server Foundations & Virtualization
**Student:** McKenzie, Cameron  
**GitHub username:** GitWitIt  
**Week:** 01  
**Date submitted:** 2025-11-03  

---

### Task / Purpose
Set up a baseline on-prem Windows Server 2019 environment to demonstrate core installation and configuration skills.

---

### Environment / Tools
- Oracle VirtualBox  
- Windows Server 2019 (Desktop Experience ISO)  
- Server Manager & Command Prompt  

---

### Steps Performed
1. Created a new VirtualBox VM (50 GB disk, 4 GB RAM, 2 cores).  
2. Installed Windows Server 2019 Desktop Experience.  
3. Renamed the computer to **Server2019-Cameron** and set an Administrator password.  
4. Enabled Remote Desktop and verified the connection.  
5. Ran `hostname && ipconfig /all` to confirm network settings.  
6. Opened Server Manager to check hostname, IP, and updates.

---

### Evidence (files in this folder)
Screenshots in the folder  

---

### Results
The Windows Server 2019 VM successfully booted and configured with verified hostname and IP.  
All features (Server Manager, Remote Desktop, and networking) function correctly.

---

### Reflection / Lessons Learned
I learned how to install and configure a baseline Windows Server VM, including naming conventions, network setup, and server verification. This provides the foundation for future Active Directory and virtualization labs.

---

### Related CLOs
CLO1, CLO5  

---

### Reproducibility Notes
Recreate by installing Windows Server 2019 Desktop Experience in VirtualBox with 4 GB RAM, 50 GB disk, and default NAT networking.
