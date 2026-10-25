# Pre Security — Network Fundamentals

## Module overview

This module introduces network communication, LANs, the OSI model, packets and frames, and methods for extending networks.

## 1. What is networking?

A network connects devices so they can exchange data and share services. Communication depends on addressing, protocols, network devices, and agreed rules.

## 2. Local Area Networks

A LAN connects devices within a limited area. A switch forwards frames within a local network, while a router forwards packets between networks. Firewalls enforce traffic rules, and wireless access points connect Wi-Fi clients.

## 3. OSI model

The seven-layer OSI model is a conceptual way to discuss networking:
1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

It helps organise troubleshooting, although real implementations are often described using the TCP/IP model.

## 4. Packets and frames

Data is encapsulated as it moves through the network stack:
- Link-layer frames support delivery on a local link.
- IP packets support addressing and routing.
- TCP segments provide reliable, ordered delivery.
- UDP datagrams provide connectionless transport.

A packet capture may show endpoints, protocol metadata, timing, and sometimes payloads, depending on encryption and capture location.

## 5. Extending a network

Routers connect networks. NAT translates addresses. Firewalls filter traffic based on policy. VPNs create protected tunnels over an underlying network. These technologies affect visibility and reachability.

## Security analyst workflow

When reviewing a network event, identify:
- Source and destination addresses
- Protocol and ports
- Timestamp and direction
- Relevant firewall, endpoint, or DNS context
- Whether the event is expected for the system and user

An IP address does not necessarily identify a person; NAT, proxies, and VPNs can affect attribution.

## Key takeaways

- Networks rely on protocols, addressing, and devices.
- OSI layers help explain where a communication issue occurs.
- Frames, packets, segments, and datagrams refer to different layers or concepts.
- Security conclusions require context and corroborating evidence.

## Rooms covered by this module

- What is Networking?
- Intro to LAN
- OSI Model
- Packets & Frames
- Extending Your Network

## Official reference

[TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity)
