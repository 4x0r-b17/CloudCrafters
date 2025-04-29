# CloudCrafters
Network Design and Infrastructure Project: Cloud Infrastructure Setup
Network Design and Infrastructure Project: Cloud Infrastructure Setup
Introduction

This project aims to design and implement a scalable and secure network infrastructure for a multi-floor office building representing a cloud-based software development company. The goal is to provide a stable, efficient, and secure network environment for multiple departments, including executives, developers, HR, IT, and cloud infrastructure teams. The network architecture includes key components such as switches, routers, firewalls, and servers, integrated with modern networking best practices like VLAN segmentation, redundancy, and security measures.
Purpose of the Project:

The main purpose of this project is to design a realistic, enterprise-level network for a cloud software company. The network must be secure, efficient, and scalable, capable of supporting different departments such as Software Development, Cloud Infrastructure, HR, and Executives. This network needs to manage internal traffic, provide internet access, isolate sensitive data, and support future growth in both users and devices.
Project Structure:

The network is designed to be multi-layered, divided into core, distribution, and access layers, with each layer serving a specific role:

    Core Layer (Floor 5): The backbone of the network, containing the Core Switch, Router, and Firewall. It serves as the central hub for inter-VLAN routing, security enforcement, and external communication with the Internet.

    Distribution Layer: The Mid-Switch 1 and Mid-Switch 2 divide the network into two logical parts — Floors 1, 2, and 3 (Mid-Switch 1) and Floors 4 and 5 (Mid-Switch 2), both of which are connected to the Core Switch. This segmentation ensures better load balancing and network redundancy.

    Access Layer: Each floor has Access Switches that connect end-user devices (e.g., PCs, VoIP phones, printers, Wi-Fi APs) and servers in isolated VLANs.

Network Design Overview

The network consists of the following components:

    Router: Provides routing between different VLANs and connects the network to the Internet.

    Firewall: Sits between the Core Router and Internet, providing network security by inspecting inbound and outbound traffic.

    Core Switch: Aggregates traffic from all Access Switches across the building and handles inter-VLAN routing.

    Mid-Switches: Distribute traffic to different floors. Mid-Switch 1 handles Floors 1, 2, and 3, while Mid-Switch 2 handles Floors 4 and 5.

    Access Switches: Connect end-user devices (PCs, phones, printers, etc.) to the network.

    Servers: Provide essential services such as Git repositories, build servers, file storage, and cloud infrastructure (located on Floors 3 and 5).

Key Elements of the Network Design:

    VLAN Segmentation:

        Different departments (HR, IT, Sales, Developers) are placed in separate VLANs to ensure traffic isolation and security.

        Voice VLAN is used to prioritize VoIP phone traffic for clearer calls.

    Redundancy:

        The network design uses redundant links between Mid-Switches and Core Switch to ensure high availability and fault tolerance.

        Dual uplinks from each Mid-Switch to the Core Switch provide failover if one link goes down.

    Security:

        Access Control Lists (ACLs) are applied to control access between VLANs and restrict unauthorized access to sensitive resources.

        Firewall rules are set to inspect and allow or block traffic based on defined security policies.

    Routing:

        Inter-VLAN Routing is done on the Core Switch or Router to allow communication between different VLANs, based on security and network policies.

    Scalability:

        The design is built to easily accommodate future expansion — more users, additional VLANs, or new floors can be added without significant changes to the core infrastructure.

Skills Involved

This project involves a broad range of networking and infrastructure skills, including but not limited to:

    Cisco Networking Configuration:

        Proficiency in using Cisco CLI for configuring VLANs, switching, routing, trunking, and ACLs.

        Knowledge of EtherChannel for link aggregation and spanning tree protocol for network loop prevention.

    Network Design:

        Creating a multi-layer network design that separates Core, Distribution, and Access layers.

        Designing for redundancy, failover, and load balancing.

    Security Configuration:

        Implementing firewalls, ACLs, and security zones to ensure the protection of sensitive data and restrict unauthorized access.

    IP Addressing and Subnetting:

        Assigning IP addresses and subnetting for each VLAN and subnet. Proper address planning ensures efficient IP utilization and scalability.

    Troubleshooting:

        Ensuring devices are connected correctly, resolving any connectivity issues, and verifying correct VLAN tagging, trunking, and routing.

    Hardware Configuration:

        Familiarity with configuring Cisco switches, routers, and firewalls.

        Connecting servers and configuring local services (DNS, DHCP, Git, file sharing, etc.).

Resources Used

    Hardware:

        Cisco Routers and Switches: Configured using Cisco 2960, 3560, and 2960X switches and Cisco routers in a Packet Tracer simulation environment.

        Firewalls: Cisco ASA (if real hardware is used).

        Servers: Simulated on virtual machines or physical servers.

        VoIP Phones: Simulated using Cisco devices in Packet Tracer.

    Software:

        Cisco Packet Tracer: For simulating network setups and configuring routers, switches, and end devices.

        GNS3/EVE-NG: Optional tools for more advanced virtual networking simulations.

        Wireshark: For packet capture and network traffic analysis.

        Linux/Windows Servers: For hosting servers like DNS, Git, Mail, and monitoring systems.

        VLAN Configuration Software: For server-side configurations (e.g., managing IPs and network resources).

    Protocols & Technologies:

        Ethernet (EtherChannel), VLANs, QoS, NAT, OSPF/EIGRP (depending on scale), RADIUS/TACACS for authentication.

        IP Routing (static/dynamic), ACLs, Firewall configuration.

Conclusion

This project successfully simulates a multi-floor, scalable network for a cloud-based software development company. It integrates critical elements such as security, redundancy, traffic management, and departmental segregation (via VLANs) to create a secure, efficient, and reliable networking infrastructure. This design is ready to scale and can accommodate future growth, including more floors, devices, and services.

Through the configuration and testing of key components, this project also highlights essential networking skills, from routing and switching to security measures and traffic prioritization. The knowledge gained in this project is applicable in real-world network administration roles, where creating a robust, scalable, and secure network is a critical requirement.
