# Day 1 - Introduction to Packet Tracer

## Overview
In this lab, we will introduce Cisco Packet Tracer, a powerful network simulation tool used for building, configuring, and troubleshooting network topologies. This tool is ideal for learning networking concepts in a hands-on way.

## Objectives
- Understand the Packet Tracer interface.
- Learn about commonly used devices in Packet Tracer.
- Set up a basic DHCP (Dynamic Host Configuration Protocol) example.

## Main Features of Packet Tracer
Packet Tracer offers several features that make it a valuable tool for both beginners and experienced network professionals:

1. **Simulation of Networking Concepts**: You can create a wide variety of network configurations to simulate real-world networking scenarios.
   
2. **Interactive Interface**: The drag-and-drop interface allows users to easily add devices, connect them, and configure their settings.

3. **Device Support**: Packet Tracer includes a variety of Cisco devices, such as routers, switches, and access points, allowing users to practice configuring these devices.

4. **Real-Time and Simulation Modes**: You can run your network in real-time to see how it behaves or switch to simulation mode to see data packets moving through the network step by step.

5. **Support for Multiple Protocols**: It supports various networking protocols, including DHCP, OSPF, RIP, and more, giving users a chance to learn about different networking technologies.

6. **Learning Resources**: Packet Tracer includes built-in tutorials and labs to help you learn various networking concepts effectively.

For more detailed information about Packet Tracer features, you can visit [Cisco Networking Academy](https://www.netacad.com/courses/packet-tracer).

## Commonly Used Devices
In Packet Tracer, you will frequently work with the following devices:

- **Routers**: These devices connect different networks and direct data packets between them. Common routers include the Cisco 7200 and 1941 models.

- **Switches**: Used to connect devices within a single network, switches like the Cisco 2960 and 3560 are essential for creating a local area network (LAN).

- **End Devices**: These include PCs, laptops, and servers. They are used to send and receive data over the network.

- **Access Points**: Used for wireless connectivity, access points allow devices to connect to the network wirelessly.

## Setting Up a Basic DHCP Example
### Steps:
1. **Open Packet Tracer**: Launch the application and create a new project.

2. **Add Devices**: Drag a router, a switch, and two PCs onto the workspace.

3. **Connect Devices**: Use the appropriate cables to connect:
   - Connect the router to the switch using a straight-through cable.
   - Connect each PC to the switch using straight-through cables.

4. **Configure the Router**:
   - Click on the router and select the CLI tab.
   - Enter the following commands to enable DHCP:
     ```bash
     enable
     configure terminal
     ip dhcp pool MYPOOL
     network 192.168.1.0 255.255.255.0
     default-router 192.168.1.1
     ```
   - This creates a DHCP pool that assigns IP addresses in the range of 192.168.1.0/24.

5. **Configure the PCs**:
   - Click on each PC and go to the Desktop tab.
   - Select IP Configuration and choose "DHCP" to obtain an IP address automatically.

6. **Test the Configuration**: Use the command prompt in the PCs to ping each other and verify the DHCP configuration.

## Images
![Packet Tracer Interface](./images/interface.png)
![Basic DHCP Setup](./images/dhcp_setup.png)

## Conclusion
Today, you learned the basics of Cisco Packet Tracer, its main features, and how to set up a simple DHCP example. Understanding these fundamentals will help you as you progress through the rest of the labs.

Feel free to explore Packet Tracer further and experiment with different configurations!

