# SOHO Network with VLAN Segmentation & Inter-VLAN Routing

This project simulates a Small Office/Home Office (SOHO) network using Cisco Packet Tracer.  
It demonstrates VLAN segmentation, trunking, inter-VLAN routing (router-on-a-stick), DHCP services, and basic switch security.

## Topology Overview

- 1 Router (Router-on-a-stick)
- 2 Switches (Layer 2)
- 3 VLANs:
  - VLAN 10 – Admin (192.168.10.0/24)
  - VLAN 20 – Sales (192.168.20.0/24)
  - VLAN 30 – Guest (192.168.30.0/24)
- Trunk links between switches and router
- DHCP on router for each VLAN
- SSH enabled for secure remote management
- Port security on access ports

## Skills Demonstrated

- VLAN and trunk configuration
- Router subinterface configuration
- Inter-VLAN routing
- DHCP configuration on Cisco router
- Basic switch security (SSH, port security)
- Network design, addressing, and documentation

## How to Use

1. Open the `soho-network.pkt` file in **Cisco Packet Tracer**.
2. Wait for devices to boot and obtain IP addresses via DHCP.
3. From a PC in each VLAN:
   - Use `ipconfig` to verify IP, subnet mask, and default gateway.
   - Ping PCs in other VLANs to verify inter-VLAN routing.
4. Use the CLI on switches/routers to run:
   - `show vlan brief`
   - `show interfaces trunk`
   - `show ip interface brief`
   - `show ip dhcp binding`

## Future Improvements

- Add ACLs to restrict traffic between VLANs.
- Add a small WAN branch and dynamic routing (OSPF).
- Add Wireshark captures to analyze traffic flows.
