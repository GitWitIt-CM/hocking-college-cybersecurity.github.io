Lab 1 – Windows Server 2019 Installation (Project 1-1)

Student: Cameron McKenzie
GitHub: GitWitIt
Date Submitted: 2025-11-03

Task / Purpose

Install Windows Server 2019 Datacenter (Desktop Experience) in a virtual environment, configure the Administrator account, verify OS details using PowerShell, and document the installation process and system information.

Environment / Tools

Oracle VirtualBox

Windows Server 2019 Datacenter (Desktop Experience) ISO

PowerShell

System Properties panel

Steps Performed

Created a new VirtualBox VM (4 GB RAM, 2 CPU cores, 50 GB virtual disk).

Attached the Server 2019 Datacenter ISO as boot media.

Booted the VM and selected:

Windows Server 2019 Datacenter (Desktop Experience)

Accepted license terms and chose Custom Install.

Deleted all partitions and installed to unallocated space.

After installation, set the Administrator password to Secret555.

Logged in to the desktop as Administrator.

Opened PowerShell and ran required commands:

systeminfo

Get-ComputerInfo | Select WindowsProductName, OsVersion, CsManufacturer, CsModel

Opened System Properties to verify OS edition and system hardware.

Evidence / Screenshots (included in this folder)

Screenshot 1: Desktop after first login

Screenshot 2: PowerShell output (systeminfo)

Screenshot 3: PowerShell output (Get-ComputerInfo)

Screenshot 4: System Properties window

Results

Windows Server 2019 Datacenter successfully installed and verified.
PowerShell confirmed correct product name, OS version, and VirtualBox hardware details.
System booted with no errors, and all required verification steps were completed.

Reflection / Lessons Learned

I learned how to perform a clean installation of Windows Server 2019, including partitioning, selecting the correct edition, setting the Administrator password, and verifying server details. Running systeminfo and Get-ComputerInfo helped me understand how to confirm OS and hardware details after deployment.

Reproducibility Notes

Recreate by installing Windows Server 2019 Datacenter (Desktop Experience) in VirtualBox using the ISO, selecting Custom Install, deleting partitions, and using password Secret555 when prompted. Then run the required PowerShell commands and capture screenshots.
