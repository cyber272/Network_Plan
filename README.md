## Network Company Documentation

This repository contains documentation for a network design project completed as part of a student assignment. Below is a detailed overview of the network design.

### 1. Diagram

The network is structured into the following segments:

- **Management**
- **Study**
- **Production 1**
- **Production 2**

![Network Diagram]()
<img width="1729" alt="Screenshot 2024-04-05 at 11 11 29" src="https://github.com/cyber272/Network_Plan/assets/155965877/78861d23-2a9f-4c92-a284-fae582c96a8d">



### 2. IP Addressing Table and VLAN

| Group       | VLAN ID | Network Address | First IP Address Available | Last IP Address Available | Default Gateway    |
|-------------|---------|-----------------|----------------------------|---------------------------|---------------------|
| Management  | VLAN 10 | 192.168.3.0/28  | 192.168.3.1                | 192.168.3.14              | 192.168.3.15        |
| Study       | VLAN 20 | 192.168.4.0/27  | 192.168.4.1                | 192.168.4.30              | 192.168.4.31        |
| Production 1| VLAN 30 | 192.168.5.0/26  | 192.168.5.1                | 192.168.5.62              | 192.168.5.63        |
| Production 2| VLAN 30 | 192.168.5.64/26 | 192.168.5.65               | 192.168.5.126             | 192.168.5.127       |
| Service     | VLAN 40 | 192.168.1.0/30  | 192.168.1.1                | 192.168.1.2               | 192.168.1.3         |

### 3. Key Devices

| Network Segment | IP Address     | Device Type                |
|-----------------|----------------|----------------------------|
| Management      | 192.168.3.1    | Router                     |
| Study           | 192.168.4.1    | Router                     |
| Production 1    | 192.168.5.1    | Router                     |
| Production 2    | 192.168.5.65   | Router                     |
| Service         | 192.168.1.3/28 | RADIUS Server / ISCSI Storage |

### 4. Service Devices

| Service           | IP Address     | Service Type          |
|-------------------|----------------|-----------------------|
| DHCP              | 192.168.10.30  | DHCP Server           |
| Active Directory  | 192.168.0.31   | Active Directory/DNS  |
| ISCSI Storage     | 192.186.1.2    | ISCSI Storage Server  |
| RADIUS            | 192.168.1.4/28 | RADIUS Server         |
| RADIUS            | 192.168.1.5/28 | RADIUS Server         |

### 5. Security Measures

- **Tree Topology**: Provides efficient scalability, flexibility, reliability, and security.
- **DMZ Implementation**: Isolates traffic using VLANs and ACLs to simulate firewall functionality in Packet Tracer.
  - Contains separate servers for storage, DNS/AD Directory, and DHCP.
  - Utilizes VLANs (trunks) and ACLs to protect servers from external network access.

### 6. Cost Breakdown of Network Components

- 2 x Routers: €1700
- 3 x Servers: €6000
- 1 x Switch 2960-24TT: €1500
- 4 x Switches 2950T-24: €2200
- 1 x Switch 3560-24PS layer 3: €1500
- 33 x Computers: €33,000
- Various Ethernet Cables: €300

**Total Cost: €38,500**

### Conclusion

This network design incorporates essential elements such as VLANs, routing, server services, and security measures within a structured and cost-effective framework.

---
