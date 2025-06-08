# basic-lan-vlan-dhcp
A basic LAN network design with VLANs and DHCP using Cisco Packet Tracer.

# Enterprise LAN Network Design with VLANs and DHCP (Cisco Packet Tracer)

## Project Overview

This project simulates an enterprise-level Local Area Network (LAN) using Cisco Packet Tracer. It demonstrates the practical implementation of network segmentation with VLANs and dynamic IP address assignment through a centralized DHCP server. The topology ensures scalability, efficiency, and logical separation of departments.

## Key Features

- **VLAN Implementation:** Logical segmentation for Sales, Marketing, and IT departments.
- **Inter-VLAN Routing:** Configured via a Multi-Layer Switch (MLS) to enable communication between VLANs.
- **DHCP Configuration:** Centralized DHCP server automatically assigns IP settings to all client devices.
- **DHCP Relay (IP Helper-Address):** Enables VLANs without direct DHCP access to receive IP addresses through relayed requests.
- **Access Layer Design:** Layer 2 switches used to connect PCs and assign ports to appropriate VLANs.



##  VLAN and IP Addressing Scheme

| VLAN ID | VLAN Name   | Subnet             | Default Gateway       |
|---------|-------------|--------------------|------------------------|
| 10      | Sales       | 192.168.10.0/24    | 192.168.10.1           |
| 20      | Marketing   | 192.168.20.0/24    | 192.168.20.1           |
| 30      | IT          | 192.168.30.0/24    | 192.168.30.1           |
| 40      | DHCP Server | 192.168.40.0/24    | 192.168.40.1           |

- **DHCP Server IP (Static):** `192.168.40.2`

## 🛠 Setup & Testing Instructions

1. **Download the Project File:**
   - `LAN Design with VLANs and DHCP.pkt`

2. **Open in Cisco Packet Tracer.**

3. **Verify Connections:**
   - Ensure green links between devices (physical connectivity).

4. **Test DHCP:**
   - On any PC → Desktop → IP Configuration → Select `DHCP`.
   - Confirm automatic IP assignment from the correct VLAN.

5. **Test Inter-VLAN Routing:**
   - `ping` devices across VLANs (e.g., PC in Sales → PC in Marketing).

6. **Test DHCP Server Reachability:**
   - `ping` from any PC to `192.168.40.2`.

##  Project Contents

- `your_project_file_name.pkt` – Cisco Packet Tracer project file.
- `LAN Design with VLANs and DHCP.jpg` – Network topology diagram.
- `README.md` – Project documentation.

##  Contribution

Feel free to suggest improvements, raise issues, or submit pull requests. Contributions are welcome.

