# LAB 3: Simulation of Network Devices Using Cisco Packet Tracer

## OBJECTIVES

- To gain a fundamental understanding of computer networking concepts using simulation software.
- To examine the internal working principles and operational logic of hardware like hubs, switches, and bridges.
- To study the roles of routers and repeaters in extending and directing network traffic.
- To analyze how data packets flow between different nodes to understand transmission patterns.
- To observe real-time communication processes and understand how various devices handle data delivery.

---

## THEORY

Cisco Packet Tracer is an interactive network simulation and visualization application used to design and analyze network topologies without relying on actual networking hardware. It is based on packet-level simulation principles, enabling users to create networks by placing virtual routers, switches, and end devices and studying how they communicate within a simulated environment.

The tool offers two operating modes:

- **Real-Time Mode** – configuration changes take effect instantly.
- **Simulation Mode** – allows users to pause network activity and examine packet movement across OSI layers.

By emulating the functionality of Cisco IOS (Internetwork Operating System), Packet Tracer bridges networking theory with hands-on practice and helps in understanding real-world network implementation.

---

## NETWORK DEVICES

### Hub

A hub is a basic physical layer device that connects multiple computers in a network. It operates on a broadcast principle—when it receives data on one port, it forwards the data to all other ports. This leads to unnecessary traffic, data collisions, and minimal security.

---

### Switch

A switch is an intelligent network device that operates at the Data Link Layer (Layer 2). It forwards data only to the intended device using MAC addresses, reducing collisions and improving efficiency and security compared to hubs.

---

### Bridge

A bridge connects or divides network segments and builds a MAC address table to filter traffic. By allowing only necessary data to cross segments, it reduces network congestion and improves performance.

---

### Router

A router is a Network Layer (Layer 3) device that routes data between different networks. It uses IP addresses and routing tables to determine the best path for packet delivery and blocks broadcast traffic between networks.

---

### Repeater

A repeater operates at the Physical Layer (Layer 1) and regenerates weak or distorted signals to extend network distance. It does not analyze or filter data—its sole purpose is signal regeneration.

---

## OBSERVATION

### Hub

**Device:** Hub-PT Hub0  

| PC Name | IP Address |
|-------|------------|
| PC0 | 192.168.1.1 |
| PC1 | 192.168.1.2 |
| PC2 | 192.168.1.3 |
| PC3 | 192.168.1.4 |

**Observation:**  
The hub acted as a central connection point and broadcasted data to all ports without identifying the intended recipient. This resulted in unnecessary traffic and frequent data collisions, demonstrating the inefficiency of hubs.

---

### Switch

**Device:** 2960-24TT Switch0  

| PC Name | IP Address |
|-------|------------|
| PC0 | 192.168.1.1 |
| PC1 | 192.168.1.2 |
| PC2 | 192.168.1.3 |
| PC3 | 192.168.1.4 |

**Observation:**  
The switch used a MAC address table to forward data only to the intended destination. This eliminated unnecessary traffic and collisions, showing why switches are preferred in modern LANs.

---

### Bridge

**Devices:**  
- Bridge-PT Bridge0  
- 2960-24TT Switch0  
- 2960-24TT Switch1  

| PC Name | IP Address |
|-------|------------|
| PC0 | 192.168.1.1 |
| PC1 | 192.168.1.2 |
| PC2 | 192.168.1.3 |
| PC4 | 192.168.1.4 |
| PC5 | 192.168.1.5 |
| PC6 | 192.168.1.6 |

**Observation:**  
The bridge filtered traffic and allowed packets to cross only when required. This reduced congestion and created smaller collision domains, improving overall network efficiency.

---

### Router

**Devices:**  
- 2960-24TT Switch0  
- 2960-24TT Switch1  
- 1941 Router2  

**Router IP Configuration:**

| Interface | IP Address |
|---------|------------|
| GigabitEthernet0/0 | 192.168.1.4 |
| GigabitEthernet0/1 | 10.10.10.4 |

**PC Configuration:**

| PC Name | IP Address |
|-------|------------|
| PC0 | 192.168.1.1 |
| PC1 | 192.168.1.2 |
| PC2 | 192.168.1.3 |
| PC4 | 10.10.10.1 |
| PC5 | 10.10.10.2 |
| PC6 | 10.10.10.3 |

**Observation:**  
The router enabled communication between two different networks using IP routing. It blocked broadcast traffic and acted as a gateway between networks, demonstrating its importance in inter-network communication.

---

### Repeater

**Devices:**  
- Repeater-PT Repeater0  
- 2960-24TT Switch0  
- 2960-24TT Switch1  

| PC Name | IP Address |
|-------|------------|
| PC0 | 192.168.1.1 |
| PC1 | 192.168.1.2 |
| PC2 | 192.168.1.3 |
| PC4 | 192.168.1.4 |
| PC5 | 192.168.1.5 |
| PC6 | 192.168.1.6 |

**Observation:**  
The repeater regenerated weakened signals over long distances, ensuring data reached the destination without loss or corruption.

---

## CONCLUSION

This experiment successfully demonstrated the working of key network devices using Cisco Packet Tracer. Hubs and repeaters operate at the Physical Layer (Layer 1) without address awareness. Switches and bridges function at the Data Link Layer (Layer 2) using MAC addresses, while routers operate at the Network Layer (Layer 3) using IP addresses. The simulation clearly showed the evolution of intelligence across networking devices.
