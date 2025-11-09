## Network Security Foundations

**Topology Name:** Threat Landscape Lab  
**Devices:**  
- Router  
- Switch  
- PC  

**CLI Commands Executed:**
```
enable
configure terminal
service password-encryption
banner motd #Authorized Access Only#
line vty 0 4
 password cisco
 login
exit
show running-config
show port-security
```
