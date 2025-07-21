# 🔐 NTI Network Security Project

This project is a complete implementation of a secure and scalable multi-area OSPF network for the NTI (Network Training Institute) course. It includes advanced routing, VLAN segmentation, AAA security, time synchronization, and centralized logging.

---

## 🌐 Project Overview

- **Main Network:** `192.168.1.0/24`
- **Subnetting:**
  - 🔹 9 LANs  
    - 8 LANs: `/29`  
    - 1 LAN: `/28`
  - 🔹 8 WAN links: `/30`
- **Routing Protocol:** OSPF (Open Shortest Path First) with MD5 authentication
- **Security:** AAA authentication using TACACS+
- **Management Services:** NTP server, Syslog server
- **Remote Access:** SSH-enabled access to all routers

---

## 🧱 Technologies Used

| Component          | Technology       |
|-------------------|------------------|
| Routing Protocol   | OSPF (multi-area)|
| Authentication     | AAA (TACACS+)    |
| VLANs              | Segmentation for LANs |
| NTP                | Time Sync        |
| Syslog             | Centralized Logging |
| Access             | SSH              |
| Tools              | Cisco Packet Tracer |

---

## 🛠️ Configured Features

- 🔐 **OSPF Routing** with proper subnet advertisements and MD5 authentication
- 👥 **AAA Authentication** using TACACS+ fallback to local
- 🧩 **VLAN-based LAN Segmentation** for structured access zones
- ⏰ **NTP Server Configuration** for accurate device clocks
- 📋 **Syslog Configuration** for event logging and monitoring
- 🔐 **SSH Remote Access** with secure user credentials
- 🌐 **WAN Connectivity** with point-to-point `/30` subnets
- 🚦 **Device Hardening** via passwords, secrets, and local user creation

---

## ✅ Completed Subnetting Plan

| Subnet Type | Quantity | CIDR   | IPs per Subnet |
|-------------|----------|--------|----------------|
| LAN         | 8        | /29    | 6 usable       |
| LAN (HQ)    | 1        | /28    | 14 usable      |
| WAN Links   | 8        | /30    | 2 usable       |

Total subnets used: **17**

---

---

## 🔎 Verification & Testing

- `ping` and `traceroute` tests across all LANs and WANs
- OSPF neighbors verified with `show ip ospf neighbor`
- NTP sync verified with `show clock`
- Syslog messages verified with `show logging`
- AAA tested via SSH login attempts
- Full IP routing table checked with `show ip route`

---

## 👨‍💻 Author

**Yehia Tarek**  
Cyber Security Student @ Alexandria National University  
NTI Network Security Trainee  
[GitHub Profile](https://github.com/yehia-dev)

---

## 📜 License

This project is developed for academic purposes as part of the NTI Network Security training.  
Unauthorized commercial use is not permitted.
