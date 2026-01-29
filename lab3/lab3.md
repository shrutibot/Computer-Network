# Lab 4: Supernetting and Subnetting

## Objectives

- To develop a thorough understanding of the principles of subnetting and supernetting through theoretical study.
- To execute these addressing techniques practically by configuring network topologies within the Cisco Packet Tracer environment.

---

## Theory

Cisco Packet Tracer is an interactive network design and simulation application that allows users to create and analyze network topologies without using real networking equipment. It is based on packet-level simulation, enabling virtual routers, switches, and end devices to be placed and configured within a simulated environment.

The tool supports two working modes:

- **Real-Time Mode** – Network devices react instantly to configuration changes.
- **Simulation Mode** – Allows users to pause network operations and closely observe the flow of packets across different OSI layers.

By emulating the functionality of Cisco IOS (Internetwork Operating System), Packet Tracer effectively bridges theoretical networking knowledge with practical, real-world configuration skills.

---

## Supernetting

Supernetting, also known as route summarization, is a networking technique used to combine multiple adjacent networks into a single larger network by applying a shorter subnet mask. It is the opposite of subnetting and is commonly implemented in routers to simplify routing tables.

Supernetting reduces the number of routing entries, improves routing efficiency, and minimizes memory usage and processing overhead.

---

## Subnetting

Subnetting is the process of dividing a single large physical network into multiple smaller logical networks called subnets. This is done by borrowing bits from the host portion of an IP address and adding them to the network portion.

The main objectives of subnetting are:
- Improving network security
- Reducing broadcast traffic
- Efficient utilization of IP addresses within an organization

---

## Device Configuration Table

| Device Type | Device Name | IP Address     | Subnet Mask     | Default Gateway |
|------------|-------------|---------------|-----------------|-----------------|
| PC-PT      | PC0         | 192.168.1.10  | 255.255.252.0  | 192.168.1.1    |
| PC-PT      | PC1         | 192.168.2.10  | 255.255.252.0  | 192.168.1.1    |
| PC-PT      | PC2         | 192.1

