# Homelab Project

A personal homelab running on VirtualBox on my HP Envy x360 2-in-1 (16GB RAM).

## What is this?

A virtualised home network I'm building to get proper hands-on experience with network security concepts in a safe, controlled setting. The goal is to bridge the gap between theoretical knowledge from my degree and actually being able to set things up, configure and troubleshoot them myself.

> Note: All IP addresses and network configurations shown in this documentation belong to private, non-routable ranges utilised within an isolated VirtualBox environment. This setup is strictly for educational, testing, and cybersecurity practice purposes.

## Current Environment

- **Host:** HP Envy x360 2-in-1, 16GB RAM
- **Hypervisor:** VirtualBox
- **VMs:**
  - pfSense (router/firewall)
  - Ubuntu 24.04 LTS (client machine)

Kali Linux will be added later as an attack machine once I get the base network between pfSense and Ubuntu up and running.

## Structure

- `progress/` - running log of what I've built, configured, broken and troubleshot
- `images/` - screenshots as I go

## Key Learnings So Far

- Planned and designed the network topology using draw.io before touching any configuration, establishing good practice of designing before building
- Configured pfSense as a router/firewall with WAN (NAT) and LAN interfaces, including manual IP addressing and DHCP pool setup
- Made deliberate IP addressing decisions to avoid conflicts with existing home network ranges
- Identified and corrected a misconfiguration in pfSense's WAN interface settings
- Verified end-to-end network connectivity between VMs and the internet through pfSense
