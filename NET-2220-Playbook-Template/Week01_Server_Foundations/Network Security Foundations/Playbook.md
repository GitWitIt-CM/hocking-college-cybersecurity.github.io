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
**Screenshots and Descriptions:**

1. ![Physical](physical.png)  
   _Shows the Physical topology layout in Packet Tracer._

2. ![Logical](logical.png)  
   _Displays the Logical network topology view with all device connections._

3. ![PortSecurity](portsecurity.png)  
   _Output of the **show port-security** command showing secured MAC addresses._

4. ![RunConfig](runconfig.png)  
   _Output of the **show running-config** command displaying configured settings._
