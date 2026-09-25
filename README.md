# ABC University Multi-Campus Network Design

## Project Overview

This project presents a multi-campus university network designed and
implemented using **Cisco Packet Tracer**.

The network connects university departments, faculties, student
laboratories, IT infrastructure, and an externally hosted email server.
The design uses VLAN segmentation, inter-VLAN routing, router-based
DHCP, RIPv2 dynamic routing, static routing, trunking, and switch
security.

## Network Topology

The network consists of a **Main Campus** and a **Smaller Health &
Sciences Campus**.

### Main Campus

#### Building A -- Administration & Business

-   Administration / Management -- VLAN 10 -- `192.168.1.0/24`
-   Human Resources -- VLAN 20 -- `192.168.2.0/24`
-   Finance -- VLAN 30 -- `192.168.3.0/24`
-   Business Faculty -- VLAN 40 -- `192.168.4.0/24`

Building A devices obtain IP addresses dynamically using a
**router-based DHCP server**.

#### Building B -- Engineering & Art

-   Engineering & Computing -- VLAN 50 -- `192.168.5.0/24`
-   Art & Design -- VLAN 60 -- `192.168.6.0/24`

#### Building C -- Student Labs & IT

-   Student Labs -- VLAN 70 -- `192.168.7.0/24`
-   IT Department -- VLAN 80 -- `192.168.8.0/24`

The IT department hosts the university web server and other internal
servers.

## Smaller Campus -- Health & Sciences

The smaller campus contains the **Faculty of Health & Sciences**. Staff
and student laboratory networks are separated using VLANs.

-   Health & Sciences Staff -- VLAN 90 -- `192.168.9.0/24`
-   Health & Sciences Student Labs -- VLAN 100 -- `192.168.10.0/24`

## Routing

### RIPv2

**RIPv2** is used for dynamic routing between the internal university
routers.

### Static Routing

Static routing is used for connectivity to the externally hosted email
server.

The external email server network is:

``` text
20.0.0.0/30
```

## VLAN and Switching

VLANs are used to separate departments and faculties into individual
logical networks.

Trunk links are configured between appropriate network devices to carry
traffic from multiple VLANs.

Switch security features such as **port security** are configured on
appropriate access ports.

## Key Features

-   Multi-campus university network
-   Three main-campus buildings
-   Health & Sciences secondary campus
-   VLAN-based network segmentation
-   Inter-VLAN routing
-   Router-based DHCP
-   RIPv2 dynamic routing
-   Static routing
-   802.1Q trunking
-   Internal university servers
-   External email server connectivity
-   Switch port security
-   End-to-end connectivity testing

## IP Addressing Plan

  VLAN   Network             Department / Faculty
  ------ ------------------- --------------------------------
  10     `192.168.1.0/24`    Administration
  20     `192.168.2.0/24`    HR
  30     `192.168.3.0/24`    Finance
  40     `192.168.4.0/24`    Business
  50     `192.168.5.0/24`    Engineering & Computing
  60     `192.168.6.0/24`    Art & Design
  70     `192.168.7.0/24`    Student Labs
  80     `192.168.8.0/24`    IT Department
  90     `192.168.9.0/24`    Health & Sciences Staff
  100    `192.168.10.0/24`   Health & Sciences Student Labs

## Technologies Used

-   Cisco Packet Tracer
-   VLANs
-   Inter-VLAN Routing
-   DHCP
-   RIPv2
-   Static Routing
-   802.1Q Trunking
-   IP Addressing and Subnetting
-   Switch Port Security
-   LAN/WAN Network Design

## Project Objectives

1.  Design a scalable university network infrastructure.
2.  Separate departments and faculties using VLANs.
3.  Assign each department/faculty a separate IP network.
4.  Provide automatic IP addressing for Building A using router-based
    DHCP.
5.  Implement inter-VLAN communication.
6.  Implement RIPv2 for internal routing.
7.  Implement static routing for the external email server.
8.  Connect the main campus with the smaller Health & Sciences campus.
9.  Apply appropriate switch security configurations.
10. Test end-to-end connectivity between users, departments, campuses,
    and servers.

## Network Diagram

The Cisco Packet Tracer topology shows the complete ABC University
network, including the main campus, three buildings, Health & Sciences
campus, routers, multilayer switching, access switches, departmental
VLANs, internal servers, external email server, and end-user devices.

## Project File

The Cisco Packet Tracer project file (`.pkt`) contains the complete
network topology and configurations.

------------------------------------------------------------------------

**Project:** ABC University Multi-Campus Network Design\
**Platform:** Cisco Packet Tracer\
**Focus:** Enterprise Networking, VLANs, Routing, DHCP & Network
Security
