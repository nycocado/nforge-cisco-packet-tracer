# NForge Network Simulation

A network infrastructure simulation for **NForge**, a company specialized in producing video cards and researching AI solutions. This project was developed using **Cisco Packet Tracer** for the "Redes e Comunicações de Dados" (Data Networks and Communications) course.

[![License: MIT](https://img.shields.io/badge/License-MIT-3da639.svg)](LICENSE)
![Status](https://img.shields.io/badge/status-completed-6f42c1)

[Portuguese](README.pt.md) | English

## About

NForge is a growing company with three main buildings: **Headquarters (Sede)**, **Factory (Fábrica)**, and **Data Center**. The project simulates the entire network topology required to support their administrative, manufacturing, and data management operations, including modern IoT integrations.

The network is designed using a **Tree Topology**, ensuring scalable and robust connectivity across all sectors.

## Features

- **Hierarchical Network Design**: Implementation of a tree topology connecting the Headquarters, Factory, and Data Center.
- **VLAN Segmentation**: Extensive use of Virtual LANs (VLANs) to separate departments and services (e.s. Management, HR, R&D, IoT, etc.).
- **Comprehensive Services**:
  - **DHCP & DNS**: Automated IP assignment and name resolution for both IPv4 and IPv6.
  - **Web Services (HTTP)**: Internal company portals.
  - **Mail Services**: Dedicated email servers for various departments.
- **IoT Integration**: Smart building management including:
  - **Temperature Control**: Automated HVAC management.
  - **Fire/Gas Detection**: Automated alarms and ventilation (CO/CO2) based on sensor thresholds.
  - **Access Control (RFID)**: Secure door management based on ID-specific permissions per building.
- **Dual-Stack Implementation**: Full support for both **IPv4** and **IPv6** protocols.

## Network Architecture

### Buildings
- **Headquarters (Sede)**: 4 floors covering administration, engineering, marketing, logistics, and HR.
- **Factory (Fábrica)**: Covers assembly, warehouse, R&D, and hardware engineering.
- **Data Center**: The backbone of the company, hosting core services (DHCP, DNS, HTTP, Mail, and IoT Registry).

### Key VLANs
| VLAN ID | Purpose |
| --- | --- |
| **20** | Servers (DHCP, DNS, Web, Mail, IoT Registry) |
| **30** | IoT Devices |
| **40-46** | Administrative sectors (HR, Finance, Marketing, etc.) |
| **60-62** | Engineering, R&D, and Factory |

## Requirements

| Tool | Minimum version |
| ---- | --------------- |
| Cisco Packet Tracer | 8.0+            |

## How to run

1. Download the simulation file (if provided).
2. Open the file in **Cisco Packet Tracer**.
3. Explore the topology to see the inter-building connectivity and IoT automation in action.

## License

Distributed under the **MIT** license, © 2024 Nycolas Souza.

It is a permissive license: anyone can use, copy, modify, and distribute the code, including in commercial projects, as long as the copyright notice and the license text are retained.

The full text is in [LICENSE](LICENSE).
