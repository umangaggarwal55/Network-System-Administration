# 🛰 Small Office Network Design – VLAN-Based Dual-Router Topology

## 📘 Project Overview

This project, titled *"Small Office Network Design", is part of the MCA curriculum (Semester 4, Subject: Network System Administration, 2023–2025) at **Chandigarh University. It demonstrates the design and implementation of a scalable, secure, and segmented enterprise network using **Cisco Packet Tracer*. Key technologies include VLANs, router-on-a-stick, RIP routing, subnetting with /26, and wireless integration.

---

## 🛠 Project Objectives

- Create 4 VLANs per router and assign them to specific switch ports.
- Use /26 subnetting for efficient address allocation.
- Implement static IP addressing for all end devices.
- Enable wireless connectivity through access points and SSIDs.
- Configure router-on-a-stick on both routers.
- Establish inter-router communication using RIP.
- Ensure seamless communication between smartphones and printers.

---
![Network Image](network%20image.jpg)


## 🧩 Network Topology Summary

| Device Type          | Quantity |
|----------------------|----------|
| Cisco Routers (2911) | 2        |
| Cisco Switches (2960)| 2        |
| PCs                  | 8        |
| Printers             | 8        |
| Wireless APs         | 8        |
| Smartphones          | 8        |
| Laptops              | 2        |

---

## 📶 VLAN & Subnet Mapping

### Router 0 (192.168.1.0/24 block)
| VLAN | Name     | Subnet           | Gateway         |
|------|----------|------------------|-----------------|
| 10   | Admin    | 192.168.1.0/26   | 192.168.1.1     |
| 20   | Finance  | 192.168.1.64/26  | 192.168.1.65    |
| 30   | CS       | 192.168.1.128/26 | 192.168.1.129   |
| 40   | Users    | 192.168.1.192/26 | 192.168.1.193   |

### Router 1 (192.168.2.0/24 block)
| VLAN | Name     | Subnet           | Gateway         |
|------|----------|------------------|-----------------|
| 50   | Admin    | 192.168.2.0/26   | 192.168.2.1     |
| 60   | Finance  | 192.168.2.64/26  | 192.168.2.65    |
| 70   | CS       | 192.168.2.128/26 | 192.168.2.129   |
| 80   | Users    | 192.168.2.192/26 | 192.168.2.193   |

---

## 🧠 Key Technologies Used

- *VLANs* for traffic segmentation and performance.
- *Router-on-a-Stick* for inter-VLAN communication.
- *RIP v2* protocol for dynamic routing between routers.
- *SSID-based Wireless Integration* per VLAN.
- *Static IP Addressing* for predictable configuration.
- *Trunking* between routers and switches.

---

## 💡 Configuration Highlights

- *Subinterfaces on Routers:* Encapsulated with dot1Q per VLAN.
- *Switch Trunk Ports:* Configured on fa0/1 for VLAN traffic tagging.
- *RIP v2 Setup:* Enables inter-router communication for all VLANs.
- *SSID Mapping:* Each VLAN has its own wireless SSID.

---

## 🧪 Testing & Troubleshooting

- Verified inter-VLAN and inter-router communication using ping.
- Troubleshooted using commands like show ip int brief, show vlan, traceroute.
- Ensured SSID-based devices (smartphones, laptops) could print across VLANs.

---

## 📂 Repository Contents

- README.md – Project summary and documentation.
- rajajajaaa.pdf – Complete project report (15 pages).
- packet_tracer.pkt – Cisco Packet Tracer simulation file (optional if available).
- /screenshots/ – Interface screenshots (optional if included).

---

## 🧑‍💻 Authors

- Umang Aggarwal  
- Sachin Singh Rawat  
- Neeraj Gupta  
- Rajat Sapehia (UID: 23MCA20474)

---

## 🏫 Institution

*University Institute of Computing*  
*Chandigarh University*

---

## 🔐 License

This project is for academic use and learning purposes. For broader usage, please credit the contributors and institution.

---

## 🔗 References

- [Cisco Networking Academy](https://www.netacad.com/)
- [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
- [Cisco Official Docs](https://www.cisco.com/)
