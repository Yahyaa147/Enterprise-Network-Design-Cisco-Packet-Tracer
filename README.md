# 🌐 High Availability & Industry 4.0 Enterprise Network Design

![Cisco Packet Tracer](https://img.shields.io/badge/Simulation-Cisco%20Packet%20Tracer-blue?style=for-the-badge&logo=cisco)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

## 📖 Project Overview
This project simulates a large-scale enterprise network infrastructure connecting three major branches: **Ankara (HQ)**, **New York**, and **Tokat**. Designed using **Cisco Packet Tracer**, the network prioritizes redundancy, security, and hierarchical design principles.

It integrates traditional networking (OSPF, HSRP, LACP) with modern **Industry 4.0 IoT automation**.

---

## 🚀 Key Features & Technologies

### 🛡️ 1. High Availability & Redundancy
* **HSRP (Hot Standby Router Protocol):** Active/Standby router configuration ensures **99.9% gateway uptime** for all VLANs.
* **LACP (EtherChannel):** Bundled links between Core Switches increase bandwidth to **2Gbps** and provide fault tolerance.
* **Dual-Homing WAN:** Primary ISP link + Backup MPLS (Serial) link ensures continuous connectivity between cities.

### 🔐 2. Advanced Security (ACLs)
* **Management Plane Protection:** Implemented **Extended ACLs** to secure critical assets.
* **Policy:** Inbound traffic from internal networks (10.x.x.x) to the Management VLAN is **BLOCKED**. Outbound traffic is permitted.
* **Port Security:** "Sticky MAC" configuration on Access Switches prevents unauthorized device access.

### 🤖 3. Industry 4.0 & IoT (Tokat Factory)
* **Smart Factory Automation:** Fully autonomous production line simulation.
* **Fire Safety System:** Smoke detectors trigger sirens, sprinklers, and open emergency exits automatically using conditional logic.

### 🌍 4. Routing & Switching Architecture
* **OSPF Area 0:** Dynamic routing protocol configured across all 3 branches for fast convergence.
* **VLAN Segmentation:** Strict isolation between Management, HR, Finance, and R&D departments using VLANs.
* **Services:** Centralized Web, DNS, Email, and DHCP servers located in the Ankara Data Center.

---

## 📂 Project Architecture Summary

| Location | Role | Key Configurations |
| :--- | :--- | :--- |
| **Ankara (HQ)** | Core & Data Center | Dual Core L3 Switches, OSPF, HSRP, Server Farm |
| **New York** | Financial Hub | Collapsed Core, LACP (EtherChannel), Dedicated Git/DB Servers |
| **Tokat** | Smart Factory | Industry 4.0 IoT Sensors, Automation Logic, Serial WAN Backup |
| **Amsterdam** | Regional Office | Router-on-a-Stick, Sub-interfaces, VLAN Routing |

---

## 📄 Detailed Documentation
For a deep dive into the configuration commands, IP addressing schemes, and detailed test results, please download the full technical report included in this repository.

👉 **[Download Full Technical Report (Document(En).docx)](Document(En).docx)**

---

## 🛠️ How to Run
1.  Download **Cisco Packet Tracer** (Version 8.0 or higher recommended).
2.  Clone this repository or download the `.pkt` file.
3.  Open `Enterprise-Network-Design-Cisco-Packet-Tracer.pkt`.
4.  Wait for OSPF convergence (green lights).

## 👨‍💻 Author
**Yahya ÖZDEN**
*Computer Networks & Data Communication Project*
