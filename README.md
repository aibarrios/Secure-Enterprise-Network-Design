# 🛡️ Secure Enterprise Network Design and Simulation

## 🛠️ Project Summary

This project simulates a complete enterprise-grade network infrastructure using Cisco switches/multiswitches and Fortinet FortiGate firewalls v7, complemented by Windows Server 2022 Standard and Ubuntu Server 24 LTS. It features a headquarter (HQ), two branch offices (BO1 and BO2), and secure remote access via IPsec VPN (FortiClient). The design emphasises high availability, centralised authentication, layered security, and scalability.

A self-directed initiative, the project showcases a secure and resilient multi-site environment that integrates routing, switching, next-generation firewalls (NGFW), zone-based segmentation, AAA via RADIUS, and complete physical and logical documentation. It closely replicates real-world deployment scenarios using enterprise technologies and commonly accepted methods for simulation, planning, and administration.

---

## 📅 Objectives

- Design and simulate a secure, scalable, and redundant enterprise network.
- Demonstrate interoperability of Cisco and FortiGate equipment with dynamic routing protocols (OSPF, BGP)
- Integrate core services (DHCP, DNS, NTP, SMB, SFTP, TFTP, RADIUS) on Windows & Ubuntu servers.
- Implement Hub-and-Spoke ADVPN for site-to-site tunnels and remote IPsec access for users.
- Harden devices with SSH, AAA (RADIUS), ACLs, VLAN, port security, DHCP snooping, and Dynamic ARP Inspection.
- Develop comprehensive network documentation, topology maps, and configurations.

---

## 📁 Repository Contents

```
.
├── Diagrams/
│   ├── Physical_Topology_AINetSec.png
│   ├── Logical_Topology_HQ.png
│   ├── Logical_Topology_BO1.png
│   ├── Logical_Topology_BO2.png
│   └── Logical_Topology_VPN.png
├── Documents/
|   ├── Network_Plan_AINetSec.docx
│   └── Secure_Enterprise_Network_Topologies.pdf
└── README.md (this file)
```

---

## 👩‍💼 Role & Responsibilities

I completed this project independently to build job-ready skills as a network engineer. This includes:

- Designing all network diagrams (physical and logical)
- Writing and applying Cisco switch, and multiswitch configurations (Layer 2, Layer 3, and security features)
- Implementing FortiGate firewall rules, routing, and VPNs
- Deploying Windows Server (AD, DNS, DHCP, NTP, SMB)
- Deploying Ubuntu Server (RADIUS, SFTP, TFTP)

---

## 🧱 Architecture Overview

- HQ acts as the IPsec ADVPN hub using FortiGate
- BO1/BO2 operate as spokes with dynamic IPsec VPN tunnels
- Cisco L2/L3 infrastructure with VLAN segmentation and inter-VLAN routing via SVIs
- Full zone-based firewall implementation across all FortiGate devices
- DMZ simulated via virtual servers (web access) using FortiGate VIP (DNAT)

---

## 🔒 Security Features

- AAA with RADIUS and local fallback (Cisco + Ubuntu Server)
- SSHv2 with ACLs and RSA key pairs (2048 bits)
- DHCP snooping, ARP inspection, and port security (sticky MACs)
- FortiGate zone-based policies with logging, DoS policies, SNAT/DNAT, Virtual Servers for DMZ
- VLAN segmentation + HSRP for gateway redundancy

---

## 🧰 Tools & Technologies Used

- **Cisco Catalyst switches** (Rapid-PVST+, Trunking with 802.1Q, HSRP, OSPFv2 with MD5, ACL, DHCP Relay, Port Security, EtherChannel with PAgP/LACP, AAA with RADIUS and local, SSHv2, Banner, VLAN + Inter-VLAN Routing with SVI, Floating and Stub Static Routes, DHCP Snooping, Dynamic ARP Inspection)
- **Fortinet FortiGate v7.0+** (Firewall Policy, DoS Policy, HA Cluster, SNAT, DNAT with Virtual Servers, SD-WAN, Default Route, Blackhole Route, OSPFv2 with MD5, BGP, IPsec VPN for Site-to-Site Hub-and-Spoke ADVPN, IPsec VPN for remote access users with FortiClient, FSSO with Windows Server)
- **Windows Server 2022 Standard** (AD, DNS, DHCP, NTP, File Share)
- **Ubuntu Server 24 LTS** (RADIUS, SFTP, TFTP)
- **VMWare Workstation Pro 17.6.2** for PNETLab Virtual Machine
- **PNETLab** for full topology simulation
- **Wireshark** for packet analysis
- **SecureCRT** for terminal emulation

---

## 🚀 Outcomes

- Developed advanced hands-on skills in network design and security
- Gained experience configuring Cisco devices and FortiGate firewalls
- Built a professional-grade project to showcase for job interviews

---

## 💼 Career Context

Although I have no prior job experience in network engineering, I hold a [**CCNA certification**](https://www.credly.com/badges/7ce7c0e3-41dc-4df0-a882-9922214a62b8/public_url) and built this project to demonstrate my real-world capabilities. This project reflects my ability to:

- Translate theory into practical network design
- Troubleshoot and configure live network devices
- Write and present professional technical documentation

---

## 🔗 Connect with Me

- [LinkedIn Profile](https://www.linkedin.com/in/aicbarrios)
- [YouTube Channel](https://www.youtube.com/@AINetSec)
- [Credly](https://www.credly.com/users/aicbarrios)
- [Explore Config Files](./Configurations)

---

Feel free to fork this project, study the configs, or reach out to collaborate or ask questions!
