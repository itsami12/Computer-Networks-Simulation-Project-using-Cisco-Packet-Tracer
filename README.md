# -----------------------------------------------------------------------------
# Enterprise Network Simulation (Cisco Packet Tracer)
# -----------------------------------------------------------------------------
# This script-style README documents a small-scale enterprise network simulation
# created in Cisco Packet Tracer. The network uses dynamic routing protocols,
# NAT, DHCP, ACLs, and more to demonstrate enterprise-grade functionality.
# -----------------------------------------------------------------------------

# -------------------------------
# 🗂️ Project Overview
# -------------------------------
# - Multi-router network topology
# - End devices: PCs, laptops, tablets, smartphones
# - Services: DHCP, Web, Email
# - Protocols: EIGRP, OSPF, RIP
# - NAT & ACLs configured
# - Layer 1 & Layer 2 tested

# -------------------------------
# 📐 Devices Used
# -------------------------------
# - 19 Cisco 2811 Routers
# - 7 Switches
# - 8 Generic PCs
# - 6 Laptops
# - 4 Smartphones
# - 2 Tablets
# - 3 Servers (DHCP, Email, Web)
# - 3 Access Points
# - 24 Copper Straight-Through Wires
# - 23 Serial Connections
# - 2 Copper Wires

# -------------------------------
# 🔧 IP Addressing
# -------------------------------
# Public IP          : 65.142.177.13
# Internal LAN       : 192.168.1.0/24
# DHCP Server        : 65.142.127.254
# Email Server       : 65.142.191.254
# Web Server         : Assigned via DHCP

# -------------------------------
# 📡 Routing Protocols
# -------------------------------
# - RIP     : Legacy zone inter-LAN routing
# - OSPF    : Internal dynamic routing (Areas 1 & 2)
# - EIGRP   : Edge routing with fast convergence
# - Static  : For specific host/network reachability
# - Redistribution: Between all routing protocols

# -------------------------------
# ⚙️ DHCP Configuration
# -------------------------------
# - DHCP server on Router R1
# - Pool includes subnet, gateway, DNS
# - Clients successfully received dynamic IPs

# -------------------------------
# 🔐 NAT & ACL Setup
# -------------------------------
# - PAT configured on Routers R8 & R20
# - Inside/outside interfaces marked
# - Verified using: show ip nat translations
# - ACL blocks: 65.143.127.255

# -------------------------------
# ✉️ Email Service
# -------------------------------
# - SMTP Server: 65.142.191.254
# - Domain: gmail.com
# - PCs configured with clients & users
# - Host-to-host mail verified

# -------------------------------
# 📁 Files
# -------------------------------
# - Project.pkt (Cisco Packet Tracer file)
# - Project Overview.docx (Full documentation)

# -------------------------------
# 🧪 Validation
# -------------------------------
# - All routers reachable via ping
# - Traceroutes tested end-to-end
# - DHCP leases confirmed
# - NAT/ACLs verified
# - Email services operational

# -------------------------------
# 🖥️ Requirements
# -------------------------------
# - Cisco Packet Tracer v7.3+ recommended

# -------------------------------
# 🚀 Usage Instructions
# -------------------------------
# $ git clone <repo-url>
# $ open Project.pkt in Cisco Packet Tracer
# $ run simulation and explore

# -------------------------------
# 📬 Contact
# -------------------------------
# Open an issue or submit a PR for questions/contributions.
