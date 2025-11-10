# RADIUS Authentication Lab — Eldar Hodzic (CI 212)

This lab demonstrates how to configure and verify a **Windows Server Network Policy Server (NPS)** for RADIUS authentication integrated with **Active Directory** and a wireless router.  
Testing was performed using a mobile device authenticating with domain credentials.

---

## Lab Overview
- **Goal:** Set up RADIUS authentication so only domain users in an authorized group can connect to the Wi-Fi network.
- **Environment:**
  - Windows Server VM running AD DS + NPS  
  - Wireless router configured as RADIUS client  
  - Mobile device connecting to the secured SSID  
  - Server IP : `192.168.0.238`

---

## Active Directory Configuration
1. Created a user account **Bill** for testing.
2. Created a security group **Wireless** for RADIUS authentication.
3. Added *Bill* to the **Wireless** group.

```text
ADUC → Users and Computers
   └── Wireless (Security Group)
         └── Bill
