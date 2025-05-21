# 🌐 Enterprise Network Simulation | Cisco Packet Tracer

![Project Type](https://img.shields.io/badge/type-Network%20Simulation-blue)
![Status](https://img.shields.io/badge/status-Completed-brightgreen)
![Tool](https://img.shields.io/badge/tool-Cisco%20Packet%20Tracer-lightgrey)
![License](https://img.shields.io/badge/license-MIT-blue)

A fully functional **small-scale enterprise network simulation** built in **Cisco Packet Tracer**. This project integrates routing protocols, DHCP, NAT, and ACLs, showcasing enterprise-level network design.

---

## 📘 Table of Contents

- [Overview](#overview)
- [Network Features](#network-features)
- [Devices & Topology](#devices--topology)
- [IP Addressing Scheme](#ip-addressing-scheme)
- [Routing Configuration](#routing-configuration)
- [Services](#services)
- [Validation](#validation)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
- [Contributing](#contributing)

---

## 🔍 Overview

This simulation demonstrates:
- Multi-area **OSPF**, **RIP**, and **EIGRP** configurations
- Advanced **NAT** and **ACL** implementation
- **DHCP**, **SMTP (Email)**, and **Web Server** configurations
- Custom IP address planning using **VLSM**

---

## 🚀 Network Features

- ✅ Dynamic & Static Routing
- ✅ PAT (Port Address Translation)
- ✅ Access Control Lists (ACLs)
- ✅ SMTP Email communication
- ✅ DHCP for automatic IP assignment
- ✅ Traceroute and end-to-end ping support

---

## 🧰 Devices & Topology

| Device Type         | Quantity |
|---------------------|----------|
| Routers (2811)      | 19       |
| Switches            | 7        |
| PCs                 | 8        |
| Laptops             | 6        |
| Smartphones         | 4        |
| Tablets             | 2        |
| Access Points       | 3        |
| Servers (DHCP, Email, Web) | 3  |
| Wires (Serial, Copper)     | ~50 |

🖼️ *A detailed topology diagram is included in the `.pkt` file.*

---

## 🧮 IP Addressing Scheme

### Core Networks:
- **Public IP**: `65.142.177.13`
- **Internal LAN**: `192.168.1.0/24`

### Key Servers:
- **DHCP Server**: `65.142.127.254`
- **Email Server**: `65.142.191.254`
- **Web Server**: Assigned via DHCP

### VLSM Summary:
- Networks segmented from `/17` to `/30`
- Separate subnet blocks for router-to-router links
- Efficient IP utilization & broadcast minimization

---

## 🔁 Routing Configuration

- 🔹 **RIP** – For legacy LAN communication
- 🔹 **OSPF (Area 1 & 2)** – Internal segmentation
- 🔹 **EIGRP** – High-speed edge routing
- 🔁 **Route Redistribution** – Between all protocols
- 🛠️ Static routes for critical path redundancy

---

## ⚙️ Services

### 📦 DHCP
- Enabled on **Router R1**
- Configured pools with gateway, subnet mask, and DNS

### 📧 Email (SMTP)
- Server IP: `65.142.191.254`
- Domain: `gmail.com`
- Clients configured with proper credentials

### 🌐 NAT
- PAT implemented on Routers **R8** and **R20**
- Verified using `show ip nat translations`
- Internal devices access internet via public IP

### 🔒 ACLs
- Access to `65.143.127.255` is blocked
- Other traffic permitted based on security policies

---

## ✅ Validation

- ✅ End-to-end **ping** and **traceroute** successful
- ✅ DHCP leases distributed and active
- ✅ NAT and ACL rules validated via CLI
- ✅ Email communication verified via Packet Tracer

---

## 💻 Requirements

- Cisco Packet Tracer **v7.3 or newer**
- Git (for cloning the repository)

---

## 📦 Getting Started

```bash
# Clone the repository
git clone https://github.com/your-username/network-simulation-packet-tracer.git

# Open the project in Cisco Packet Tracer
# Navigate to the Project.pkt file
