# Connect and Configure a LAN — Cisco Packet Tracer

## Overview

This lab focuses on building and configuring a small office Local Area Network (LAN) using Cisco Packet Tracer.

The objective is to connect network devices, configure IPv4 addressing, verify connectivity, and use networking commands to troubleshoot basic connectivity issues.

## Objectives

- Connect network devices and end hosts.
- Configure PCs to obtain IPv4 addresses through DHCP.
- Configure a static IPv4 address for a network printer.
- Verify local connectivity using `ping`.
- Inspect network settings using `ipconfig` and `ipconfig /all`.
- Trace the network path to a remote server using `tracert`.
- Verify access to a remote server by IP address and URL.

## Network Components

- Office router
- Network switch
- Admin PC
- Manager PC
- Network printer
- Internet server

## Key Networking Concepts

### IPv4 Addressing

IPv4 addresses identify devices at the network layer. Devices in the same subnet can communicate directly over the local network when their addressing and connectivity are configured correctly.

### DHCP

Dynamic Host Configuration Protocol (DHCP) automatically provides clients with network configuration, including an IP address, subnet mask, default gateway, and DNS server information.

### Default Gateway

A default gateway allows a host to send traffic to destinations outside its local subnet. In this lab, the office router provides the gateway for the PCs.

### DNS

Domain Name System (DNS) resolves domain names to IP addresses. If a website is accessible by IP address but not by URL, DNS resolution is one of the first things to investigate.

### Network Troubleshooting

- `ping` tests whether a destination responds to ICMP echo requests.
- `ipconfig` displays basic IP configuration.
- `ipconfig /all` displays detailed network adapter information.
- `tracert` helps identify responding network hops toward a destination.

## Verification

The lab includes the following verification steps:

- Check that network links are active.
- Verify that the PCs obtain their IPv4 configuration through DHCP.
- Test connectivity between the PCs and the printer using `ping`.
- Test access to the remote server by IP address and URL.
- Inspect network configuration using `ipconfig` and `ipconfig /all`.
- Use `tracert` to examine the path toward the remote server.

## Screenshots and Verification

### 1. Network Topology

The topology shows the office router, switch, Admin PC, Manager PC, printer, and connection to the internet.

![Network Topology](screenshots/01-network-topology.png)

### 2. IPv4 Configuration

This screenshot documents the IPv4 configuration of an end device, including its IP address, subnet mask, default gateway, and DNS settings.

![IP Configuration](screenshots/02-ip-configuration.png)

### 3. Local Connectivity Test

This screenshot shows the `ping` test used to verify connectivity between a PC and the printer.

![Connectivity Test](screenshots/03-connectivity-test.png)

### 4. Internet Connectivity

This screenshot documents the test of access to the remote server.

![Internet Connectivity](screenshots/04-connectivity-to-the-internet.png)

### 5. Traceroute Analysis

The `tracert` command is used to examine the network path toward the remote server and identify responding intermediate hops.

![Traceroute Output](screenshots/05-tracert-output.png)

### 6. Final Lab Result

Additional evidence from the completed lab.

![Final Lab Result](screenshots/06-result.png)

## SOC Analyst L1 Relevance

Understanding network fundamentals is important for investigating network-related security alerts.

Skills practiced in this lab are relevant to:

- Identifying source and destination IP addresses.
- Understanding DHCP and DNS behavior.
- Recognizing the role of a default gateway.
- Performing initial network connectivity checks.
- Understanding the basic network path between a host and a remote destination.

These concepts provide a foundation for further work with network logs, security monitoring, and incident investigation.

## What I Learned

- How devices connect within a small office LAN.
- How DHCP provides IPv4 configuration to client devices.
- Why hosts in the same subnet can use the same subnet mask and default gateway while having different IP addresses.
- How to test connectivity using `ping`.
- How to inspect network settings using `ipconfig` and `ipconfig /all`.
- How to use `tracert` to investigate the path toward a remote server.
- Why DNS resolution matters when accessing services by domain name.

## Tools

- Cisco Packet Tracer
- Cisco Networking Academy learning materials
- Command-line networking tools available in Packet Tracer

## Disclaimer

This repository documents my personal learning and practical lab work. Cisco and Cisco Networking Academy are the respective owners of their trademarks and course materials. This project is not affiliated with or endorsed by Cisco.
