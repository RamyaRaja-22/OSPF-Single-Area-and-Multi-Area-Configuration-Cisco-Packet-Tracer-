# OSPF Single Area and Multi-Area Configuration

## Project Overview
This project demonstrates the implementation of Open Shortest Path First (OSPF) routing protocol using both single area and multi-area configurations. The network topology is designed and simulated using Cisco Packet Tracer to understand how OSPF enables dynamic routing and efficient communication between multiple networks.

## Objectives
- Configure OSPF in a single area network.
- Implement multi-area OSPF routing.
- Understand how routers exchange routing information.
- Analyze routing tables and network connectivity.

## Technologies Used
- Cisco Packet Tracer
- OSPF Routing Protocol
- IP Addressing and Subnetting
- Router and Switch Configuration

## OSPF Single Area
In single area OSPF, all routers are placed within one OSPF area (Area 0). This allows routers to share routing information efficiently within the same area.

### Features
- Simple configuration
- Faster routing updates
- Suitable for small networks

## OSPF Multi-Area
In multi-area OSPF, the network is divided into multiple areas to improve scalability and performance. Area 0 acts as the backbone area connecting other areas.

### Features
- Reduces routing table size
- Improves network performance
- Supports large-scale networks

## Network Topology
The project includes multiple routers connected with different networks to demonstrate both single-area and multi-area OSPF configurations.

## Configuration Steps
1. Assign IP addresses to router interfaces.
2. Enable OSPF routing protocol.
3. Configure OSPF network statements.
4. Assign routers to specific OSPF areas.
5. Verify routing using routing table commands.

Example configuration:

```
router ospf 1
network 192.168.1.0 0.0.0.255 area 0
network 192.168.2.0 0.0.0.255 area 1
```

## Verification Commands
- `show ip route`
- `show ip ospf neighbor`
- `show ip protocols`

## Advantages of OSPF
- Fast convergence
- Supports hierarchical network design
- Efficient use of bandwidth
- Scalable for large enterprise networks

## Conclusion
This project helps in understanding how OSPF works in both single area and multi-area environments. It demonstrates dynamic routing, improved network performance, and efficient routing management using OSPF in Cisco Packet Tracer.
