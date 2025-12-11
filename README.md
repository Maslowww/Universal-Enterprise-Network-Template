#  Universal Enterprise Network Template

![Cisco Packet Tracer](https://img.shields.io/badge/Cisco-Packet%20Tracer-blue?style=for-the-badge&logo=cisco)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Stable-success?style=for-the-badge)

##  Overview
**This is the ultimate network infrastructure template designed for versatility and scalability.**

Whether you are studying for CCNA/CCNP, designing a corporate network, or need a robust base for cybersecurity simulations, this project covers it all. It implements industry-standard protocols for redundancy, security, and efficiency, making it suitable for **any** small to medium-sized enterprise scenario.

> *"One topology to rule them all."* — This project can be used as a foundation for virtually any network deployment task.

##  Key Features
This topology is not just a simple network; it's a fully configured enterprise environment featuring:

*   **High Availability & Redundancy:**
    *   **HSRP (Hot Standby Router Protocol):** Dual-router setup (Active/Standby) ensuring 100% uptime for the default gateway [memory:11].
    *   **EtherChannel (PAgP & LACP):** Link aggregation between Core switches and Routers for increased bandwidth and fault tolerance [memory:11].
    *   **STP (Rapid PVST+):** Loop prevention with fast convergence times.
*   **Advanced Switching:**
    *   **VLAN Segmentation:** Full separation of traffic (Management, Voice, Data departments).
    *   **Inter-VLAN Routing:** Configured on a "Router-on-a-Stick" model.
*   **Services & Security:**
    *   **VoIP Ready:** Configured Voice VLANs and IP Phones.
    *   **DHCP Pools:** Automated IP addressing for all subnets.
    *   **Security:** Port Security, SSH access, and encrypted passwords.
    *   **WAN Simulation:** Cloud connectivity simulation for remote access scenarios.

##  Topology Map
<img width="1591" height="698" alt="image" src="https://github.com/user-attachments/assets/d115a855-2a59-47fb-abb6-bd1e14004f62" />

The network follows a **Collapsed Core architecture**:
1.  **Core Layer:** Two interconnected Cisco 2960 switches acting as the high-speed backbone.
2.  **Routing Layer:** Two Cisco PT8200 routers providing WAN access and HSRP redundancy.
3.  **Access Layer:** Dedicated switches for various departments (Finance, Executive, Reception, etc.) connected via redundant links.

*(See the `topology_image.jpg` in the repository for a visual diagram)*

##  How to Use
This `.pkt` file is a "plug-and-play" template.

1.  **Clone the repo:**
    ```
    git clone https://github.com/YOUR_USERNAME/Universal-Enterprise-Network-Template.git
    ```
2.  **Open in Packet Tracer:** Ensure you have Cisco Packet Tracer (version 8.0 or newer recommended).
3.  **Customize:**
    *   Simply rename the VLANs to match your organization.
    *   Adjust the IP schema in the router configuration if needed.
    *   The infrastructure is ready to scale — just add more Access switches!

##  Contents
*   `Project_File.pkt` - The complete, pre-configured network simulation.
*   `topology.jpg` - Visual diagram of the network connections.
*   `README.md` - Documentation.

## 🎓 Perfect For
*   **Network Engineers:** A quick boilerplate for testing configs.
*   **Students:** A comprehensive lab for learning HSRP, EtherChannel, and VLANs.
*   **Cybersecurity Pentesters:** A realistic target network for Red Team practice.

---
*Created by Ihor Maslovskyi
