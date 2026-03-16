# Enterprise Network Design & Switching Lab
[<image-card alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" ></image-card>](https://opensource.org/licenses/MIT)
[<image-card alt="Networking Project" src="https://img.shields.io/badge/Project-Networking-blue" ></image-card>](https://github.com/RamtinMogh/Enterprise-Network-Design-Switching-Lab)
[<image-card alt="Aruba Switches" src="https://img.shields.io/badge/Tech-Aruba%20Switches-green" ></image-card>](https://www.arubanetworks.com/)

A hands-on group project (with teammate Sidney Mills) demonstrating enterprise-level network design and configuration. We used physical Aruba switches connected via patch panels to lab computers, with Oracle VirtualBox running Ubuntu VMs for endpoints. Key features include VLAN segmentation, trunking with LACP port channels, DHCP server setup, inter-VLAN routing, SSH connectivity, a simple hosted webpage, and traffic analysis with Wireshark.

This project highlights practical skills in network administration, troubleshooting, and security, ideal for entry-level IT/networking roles.

## Project Goals
- Design and implement a segmented network with two VLANs (48 and 62) for isolated traffic.
- Configure trunk ports with allowed VLANs and LACP for redundancy.
- Set up DHCP pools for dynamic IP assignment in each subnet (172.20.12.0/25 and 172.20.15.0/25).
- Enable inter-VLAN routing and verify connectivity via SSH and HTTP.
- Analyze network traffic using Wireshark to capture TCP handshakes for SSH (port 22) and web access (port 80).
- Use Packet Tracer only for topology visualization.

## Technologies Used
- Hardware: Aruba switches, patch panels, lab PCs.
- Software: Oracle VirtualBox, Ubuntu VMs, Wireshark.
- Protocols/Features: VLANs, Trunking (802.1Q), LACP, DHCP, STP (Spanning Tree Protocol), SSH, HTTP.

## Implementation
The network was built using real hardware and VMs. For the switch configuration scripts used to replicate the setup, see the [configs/](configs/) folder.

For full evidence including screenshots of command outputs (ip a, ip route, show ip int br, show vlan, show spanning-tree, DHCP leases), SSH connections, webpages, Wireshark captures, and the network diagram, download the PDF in the [project-evidence/](project-evidence/) folder.

## Challenges and Learnings
- Troubleshooting trunk negotiation between Aruba switches.
- Ensuring STP priority for loop prevention.
- Setting up VMs in VirtualBox for real hardware integration.
- Gained experience in physical cabling with patch panels.

## Contributions
- Ramtin Moghaddam: Switch config, DHCP setup, VM setup, Wireshark analysis.
- Sidney Mills: Switch config, STP tuning, webpage hosting.

## Repository Structure
- `configs/`: Switch configuration scripts.
- `project-evidence/`: Full project PDF with screenshots and outputs.
