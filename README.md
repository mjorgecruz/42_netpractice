# Net Practice

This repository contains a summary of the acquired knowledge after completing netpractice project.
The project focuses on understanding and configuring basic networking concepts, such as IP addressing, subnetting, and routing, to solve a series of network configuration scenarios. This README provides an overview of the project requirements and the fundamental networking concepts needed to complete it successfully.

## Introduction

The NetPractice project is designed to teach students the essential concepts of computer networking. The project consists on different exercise where we are required to configure network settings for a variety of devices in different network topologies to ensure they can communicate effectively. </br></br>

The project scenarios will test your knowledge of IP addressing, subnetting, routing, and network address translation (NAT). By completing this project, you will gain a deeper understanding of how networks are structured and how data is routed between devices.</br></br>

## IP Addressing

### IPv4 Addressing
- An IPv4 address consists of four octets (e.g., 192.168.1.1), each ranging from 0 to 255.
- Public IP Addresses:
    - A public IP address is assigned to a device that is directly accessible over the internet. It is globally unique, meaning no two devices on the internet can have the same public IP address.
    - Public IP addresses are used by servers, websites, and any devices that need to be directly reachable over the internet.
- Private IP Addresses:
    - A private IP address is used within a local network and is not directly accessible over the internet. Devices within the same local network use private IP addresses to communicate with each other.
    - Private IP addresses are reserved and defined by the following ranges:
      - **Class A:** `10.0.0.0` to `10.255.255.255` (16,777,216 addresses)
      - **Class B:** `172.16.0.0` to `172.31.255.255` (1,048,576 addresses)
      - **Class C:** `192.168.0.0` to `192.168.255.255` (65,536 addresses)
- Why the Distinction Matters:
    - *Security:** Devices with private IP addresses are isolated from direct internet access, providing a layer of security against external attacks.
    - *Address Conservation:** Using private IP addresses allows multiple devices to share a single public IP address through mechanisms like Network Address Translation (NAT), conserving the limited pool of available public IP addresses.

### Classful Addressing
- Different IP classes (A, B, C) and their default subnet masks.
    - Class A: 1.0.0.0 to 126.0.0.0 with a default subnet mask of 255.0.0.0.
    - Class B: 128.0.0.0 to 191.255.0.0 with a default subnet mask of 255.255.0.0.
    - Class C: 192.0.0.0 to 223.255.255.0 with a default subnet mask of 255.255.255.0.

## Subnetting

- Subnetting is the process of dividing a large network into smaller, manageable sub-networks (subnets). Each subnet has a specific range of IP addresses, defined by the subnet mask.
- Subnet Masks: A subnet mask determines which portion of an IP address is the network part and which is the host part (e.g., 255.255.255.0).
  
- Network Address:
   - The network address is the first address in a subnet. It identifies the subnet itself and cannot be assigned to any individual device within the subnet.
   - It helps in identifying the subnet and is essential for routing purposes.
- Broadcast Address:
   - The broadcast address is the last address in a subnet. It is used to send data to all devices within the subnet simultaneously.
   - It allows communication with all devices in a subnet, useful for network-wide announcements and services like DHCP.

## Routing

- Default Gateway:
  - The default gateway is the IP address of a router that routes traffic from a local network to other networks or the internet.
  - Devices use the default gateway to communicate with devices outside their local subnet.

- Static and Dynamic Routing:
  - Static routing involves manually setting up routes in a router.
  - Dynamic routing uses protocols (e.g., RIP, OSPF) to automatically update routing tables.

- Routing Tables:
  - Understand how routing tables determine the path for data packets based on the destination IP address.
  - Learn to read and interpret routing tables to understand how data is forwarded within a network.

