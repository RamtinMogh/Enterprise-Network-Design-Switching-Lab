# Enterprise Network Design & Switching Lab
<a href="https://www.arubanetworks.com/"><img src="https://amt-it.com/wp-content/uploads/2020/10/Aruba_Networks-Logo.wine_.png" alt="Aruba" height="30"></a>
<a href="https://www.wireshark.org/"><img src="https://www.wireshark.org/_astro/wca.C_vSXqTJ_Z2pt6cI.webp" alt="Wireshark" height="30"></a>
<a href="https://www.virtualbox.org/"><img src="https://1000logos.net/wp-content/uploads/2020/08/VirtualBox-Logo-2009.png" alt="VirtualBox" height="30"></a>
<a href="https://ubuntu.com/"><img src="https://res.cloudinary.com/canonical/image/fetch/f_auto,q_auto,fl_sanitize,c_fill,w_1920/https%3A%2F%2Fubuntu.com%2Fwp-content%2Fuploads%2Fff30%2Flogo_thumbnailYT.png" alt="Ubuntu" height="30"></a>
<a href="https://en.wikipedia.org/wiki/Virtual_LAN"><img src="https://cdn.prod.website-files.com/65f7f0027cb1900111ab2e6f/681b52b90fb1761636d217f6_Blogartikel-Bilder-2025_VLAN_1580x970px.webp" alt="VLAN" height="30"></a>
<a href="https://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol"><img src="https://www.shutterstock.com/shutterstock/photos/1860158311/display_1500/stock-vector-dhcp-dynamic-host-configuration-protocol-acronym-business-concept-word-lettering-typography-1860158311.jpg" alt="DHCP" height="30"></a>
<a href="https://en.wikipedia.org/wiki/Secure_Shell"><img src="https://ded9.com/wp-content/uploads/2022/07/ssh.png-hamyarit.com-ssh.png.webp" alt="SSH" height="30"></a>

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
