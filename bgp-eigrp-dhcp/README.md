# Multi-Site Enterprise Routing Lab (BGP, EIGRP, DHCP & VLANs)

## 📌 Purpose
Simulates a multi-site enterprise network to practice bridging interior routing protocols with border gateway routing, VLAN segmentation, and automated IP allocation.

## 🏗️ Topology Architecture
The topology connects two network zones via Cisco 2911 routers and Catalyst 2960 switches.

![Topology Diagram](bgp-eigrp-topology.png)

* **Interior Routing (EIGRP):** AS 100 configured for fast internal convergence.
* **Exterior Routing (BGP):** Peer routing established between core boundary routers.
* **VLAN Segmentation:** Layer 2 access ports and trunking linked to router subinterfaces (`802.1Q`).
* **Dynamic Addressing:** Router-based DHCP pools for automated end-device allocation.

## 💡 Key Learnings
* **Protocol Redistribution:** Bridging EIGRP and BGP routing domains for inter-domain communication.
* **Router-on-a-Stick:** Implementing subinterfaces on a single physical port for multiple VLANs (`VLAN 10` and `VLAN 20`).
* **DHCP Configuration:** Managing pools and excluded address ranges to prevent gateway conflicts.
* **Troubleshooting:** Resolving subnet alignments, link states, and verifying path availability via CLI.
