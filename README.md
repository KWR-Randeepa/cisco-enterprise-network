# Secure Enterprise Network Design — Cisco Packet Tracer

## Project Overview

This project demonstrates an enterprise network designed and simulated in Cisco Packet Tracer. It connects a head office, a branch office, and a simulated ISP network, with departmental segmentation and basic network security.

## Network Topology

![Enterprise Network Logical Diagram](docs/network-topology.png)

The topology includes three routers, two switches, five PCs, and two servers.

## Technologies

- VLANs and 802.1Q trunking
- Inter-VLAN routing
- DHCP
- OSPF dynamic routing
- Extended Access Control Lists (ACLs)
- NAT/PAT
- DNS and HTTP services
- Network troubleshooting and verification

## VLAN and IP Addressing

| Department | VLAN | Network | Default Gateway |
|---|---:|---|---|
| HR | 10 | 192.168.10.0/24 | 192.168.10.1 |
| IT | 20 | 192.168.20.0/24 | 192.168.20.1 |
| Finance | 30 | 192.168.30.0/24 | 192.168.30.1 |
| Guest | 40 | 192.168.40.0/24 | 192.168.40.1 |
| Servers | 50 | 192.168.50.0/24 | 192.168.50.1 |
| Branch | — | 192.168.60.0/24 | 192.168.60.1 |

## Security Design

The Guest VLAN is restricted from accessing the internal HR, IT, Finance, Server, and Branch networks. Public services are hosted on a separate simulated network.

## Repository Contents

- `Enterprise_Network.pkt` — Packet Tracer simulation
- `docs/` — Logical network diagram
- `configs/` — Router and switch configurations
- `screenshots/` — Network and verification evidence

## Verification Checklist

- [ ] VLANs and trunking verified
- [ ] DHCP address allocation verified
- [ ] Inter-VLAN routing verified
- [ ] OSPF adjacency and learned routes verified
- [ ] Guest ACL restrictions tested
- [ ] NAT/PAT translations verified
- [ ] Internal and public web services tested

**Test status:** Update this checklist after verifying each item in Cisco Packet Tracer.

## Lab Limitations

This is a simulated learning environment. The public IP ranges are reserved documentation ranges and represent an example ISP network, not a connection to the real internet.

## Learning Outcomes

This project provides hands-on practice in enterprise network design, IP addressing, routing, switching, network segmentation, access control, and troubleshooting.

## Tools

- Cisco Packet Tracer
- Cisco IOS CLI
- GitHub
