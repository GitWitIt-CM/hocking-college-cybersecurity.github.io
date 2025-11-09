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
![Physical](Network%20Security%20Foundations/physical.png)
![Logical](Network%20Security%20Foundations/logical.png)
![PortSecurity](Network%20Security%20Foundations/portsecurity.png)
![RunConfig](Network%20Security%20Foundations/runconfig.png)
