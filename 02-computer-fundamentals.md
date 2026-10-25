# Pre Security — Computer Fundamentals

## Module overview

Computer fundamentals explain the components that process and store information, how computer types differ, how clients and servers communicate, and how virtualisation and cloud services are used.

## 1. Inside a computer system

- **CPU:** Executes instructions and calculations.
- **RAM:** Temporarily stores data and instructions currently in use.
- **Storage:** Retains data when power is off.
- **Motherboard:** Connects components.
- **Network interface:** Enables network communication.
- **Input/output devices:** Let systems receive or present information.

The CPU, memory, storage, and I/O work together. Performance and security depend on the full system.

## 2. Computer types

Computers may be personal devices, servers, embedded systems, mobile devices, or specialised appliances. Their purpose, resource profile, physical exposure, and operating environment influence their security needs.

## 3. Client-server basics

A client requests a resource or service; a server processes the request and returns a response. A browser and web server are a common example.

Simplified flow:
1. Client prepares a request.
2. Network carries it to the server.
3. Server processes the request.
4. Server sends a response.
5. Client interprets the result.

## 4. Virtualisation

Virtualisation allows multiple virtual machines to share physical hardware through a hypervisor. It supports isolated labs, testing, snapshots, and running different operating systems on one host.

Virtual machines still require patching, access control, and appropriate network isolation.

## 5. Cloud computing

- **IaaS:** Infrastructure such as virtual machines and networks.
- **PaaS:** Managed platform for developing and running applications.
- **SaaS:** Software delivered as a service.

Security responsibility is shared between provider and customer, with the boundary depending on the service.

## Security relevance

These concepts help an analyst determine which host or service may be involved, understand where data is processed, and reason about the path between a client and a server.

## Key takeaways

- Computer components have distinct roles.
- Client-server architecture underpins many applications.
- Virtualisation provides useful isolation but does not remove security responsibilities.
- Cloud security depends on the service model and shared responsibilities.

## Rooms covered by this module

- Inside a Computer System
- Computer Types
- Client-Server Basics
- Virtualisation Basics
- Cloud Computing Fundamentals

## Official reference

[TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity)
