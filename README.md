## SOHO Network Design

### Introduction

This project involved designing and implementing a secure, high-performance, and scalable network infrastructure using Cisco Packet Tracer. A hierarchical network design was deployed with redundant core, distribution, and access layers, supporting VLAN segmentation for five departments, VoIP services, wired and wireless connectivity, and inter-VLAN routing. The solution integrates dual ISPs for redundancy and load balancing, OSPF for dynamic routing, NAT/PAT for internet access, and a site-to-site IPsec VPN to securely connect the headquarters to an external server site hosting DHCP, DNS, Web, and Email services. Security controls such as ACLs, SSH, port security, and VPN policies were implemented to ensure confidentiality, integrity, and availability of network resources, with full testing conducted to verify end-to-end communication.

### Network Diagram
<img width="816" height="718" alt="image" src="https://github.com/user-attachments/assets/c6b847f6-6973-4e5b-b09a-dbbd4eb99752" />

### Tasks
1. Hierarchical Design- Use a hierarchical model providing redundancy at every layer.
2. ISPs- The network is also expected to connect to at least two ISPs to provide redundancy and each router is connected to the two ISPs.
3. WIFI- Each department is required to have a wireless network for the users.
4. VoIP- Each department should have IP phones and users in the department should be able to call each other.
5. VLAN- Each department should be in a different VLAN and a different subnetwork. The voice VLAN ID number will remain at VID 120 for the entire network.
6. Subnetting- Provided the networks above, carry out subnetting to allocate the correct number of IP addresses to each department.
7. Basic settings- Configure basic device settings such as hostnames, and console passwords, enable passwords, and banner messages, encrypt all passwords and disable IP domain lookup.
8. Inter-VLAN Routing- Devices in all the departments are required to communicate with each other with the respective multilayer switch configured for inter-VLAN routing.
9. Core Switches- The Multilayer switches are expected to carry out both routing and switching functionalities and thus will be assigned IP addresses.
10. DHCP Server- All devices in the network (except IP phones) are expected to obtain an IP address dynamically from the dedicated DHCP servers located at the server-side site.
11. Cisco 2811 Router- Ensure to have a router that can support telephony service i.e Cisco Catalyst 2811(the VoIP router should be connected to any of the l3-switches at HQ).
12. Static Addressing- Devices in the server room are to be allocated IP addresses statically.
13. Telephony Service- Configure VoIP on the voice gateway router and allocate dial numbers in format (4..).
14. Routing Protocol- Use OSPF as the routing protocol to advertise routes both on the routers and multilayer switches.
15. Switchport security- Configure port security for the server site department switch to allow only one device to connect to a switch port, and use the sticky method to obtain mac-address and violation mode shutdown.
16. SSH- Configure SSH in all the routers and layer three switches for remote login.
17. Standard ACL for SSH- configure a simple standard ACL on the line VTY to allow only the ICT department to carry out all remote administrative tasks using SSH.
18. NAT + ACL- Configure PAT to use the respective outbound router interface IPv4 address, and implement the necessary ACL rule.
19. IPsec VPN + ACL- Configure site-to-site IPsec VPN between the HQ router and the Server-side router, and implement the necessary ACL rule.
20. Final- Test Communication, ensure everything configured is working as expected.



