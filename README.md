# PisoWifi-Network-Enumaration
A technical study of public captive portal architecture and device discovery.


##  1. Authorization & Ethics
**CRITICAL:** This project was conducted with the **explicit verbal permission** of the network owner.
- **Scope:** Local subnet discovery and service identification only.
- **Rules of Engagement:** No disruption of service, no bypass of captive portals, and no unauthorized access to client data.

##  2. My Setup
- **Host OS:** Zorin OS 17.3 (Primary Security Workstation)
- **Scanning Engine:** Nmap (Network Mapper)
- **Visualization:** Zenmap GUI
- **Environment:** Live Physical Public WiFi Network

##  3. Methodology
I utilized **Zenmap on Zorin OS** to perform a non-intrusive scan to identify how many users were active and what services the router was running.

1. **Host Discovery:** Performed a "Ping Sweep" to see active devices.
2. **Service Mapping:** Identified open ports (80/443) used for the login portal.

##  4. Results
<img width="1365" height="746" alt="image" src="https://github.com/user-attachments/assets/25ecd9e9-6610-437c-9e68-ce710ff7e6db" />
<img width="1365" height="746" alt="image" src="https://github.com/user-attachments/assets/65f91af0-8915-41a2-8e66-bfeef8d15092" />


### Findings Table
| Target IP | Status | Role |
| :--- | :--- | :--- |
| 192.168.1.1 | Online | Gateway (Piso WiFi Router) |
| 192.168.1.xx | Online | Standard Client (Mobile/PC) |
| 192.168.1.xx | Online | Standard Client |
| 192.168.1.xx | Online | Standard Client |
| 192.168.1.xx | Online | Standard Client |
| 192.168.1.xx | Online | Standard Client |
| 192.168.1.xx | Online | Filtered Device (Possible PC with Firewall) |
| 192.168.1.xx | Online | Standard Client |
| 192.168.1.xx | Online | My Zorin OS Laptop |


##  5. Security Reflection
This exercise shows that public networks are inherently "noisy." Any user on the Piso WiFi can see who else is connected. This highlights the importance of using a **VPN** or **Encrypted Protocols** when using public internet.
