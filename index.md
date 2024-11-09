---
layout: default
title: "Home"
---

# Welcome to cwsecur1ty Documentation Hub
Documenting my projects & homelab.

## Sections
- [Homelab Setup](homelab.md)
- [Administration](administration.md)
- [Security Testing & Tools](security.md)

# Welcome to the cwsecur1ty Documentation Hub

This hub documents the design, setup, and ongoing projects of my homelab & security projects. Here, you’ll find resources on each part of my Proxmox-based homelab, covering network configuration, services, monitoring, and future project plans.

---

## 📖 Table of Contents

1. [Overview](#overview)
2. [Network Setup](#network-setup)
3. [Installed Services](#installed-services)
4. [Server Architecture](#server-architecture)
5. [Security and Monitoring](#security-and-monitoring)
6. [Future Projects](#future-projects)

---

## Overview

My home lab is built on Proxmox and is designed to host various services for IT support and cybersecurity learning, experimentation, and documentation. This documentation hub will also feature network diagrams, architecture overviews, and configuration steps for anyone interested in replicating or learning from this setup.

---

## 🖧 Network Setup

The network setup involves a segmented architecture that allows for isolated environments for different services, improving both organization and security. Key elements include:

- **Virtual LANs (VLANs)**: Used to separate environments (e.g., main, lab, DMZ).
- **Firewall Rules**: Configured to restrict access and control traffic between VLANs.
- **Router Configuration**: Setup details for the network’s gateway, DNS, and DHCP.
  
➡️ [Learn more about the Network Setup](network.md)

---

## ⚙️ Installed Services

This homelab hosts several essential services for IT support and cybersecurity experimentation:

- **Proxmox Virtualization**: Foundation of the homelab, providing resource allocation and VM management.
- **SIEM Tools (Splunk, ELK Stack)**: Set up for log aggregation, analysis, and security monitoring.
- **Pihole**: Network-level ad blocker for network security and monitoring.
- **Docker and Containers**: Hosting various services in isolated environments.
  
➡️ [Explore the Installed Services](services.md)

---

## 🖥️ Server Architecture

The physical and virtual architecture includes several components designed to optimize performance, scalability, and redundancy. 

- **Proxmox Hosts**: Details on virtualized servers, including memory, CPU, and storage allocation.
- **Storage Solutions**: Setup of storage for VM and container volumes.
- **Backups and Snapshots**: Regular backups and snapshots to ensure quick recovery in case of failures.

➡️ [View the Server Architecture](architecture.md)

---

## 🔒 Security and Monitoring

Security is a priority in this homelab, with multiple tools and processes in place for monitoring and threat detection.

- **Firewall and Intrusion Detection**: Configuration of firewalls and IDS/IPS tools.
- **SIEM Analysis**: Using Splunk and the ELK Stack for real-time log analysis.
- **Network Monitoring**: Tools like Zabbix or Nagios to keep track of network and server health.

➡️ [Dive into Security and Monitoring](security.md)

---

## 🚀 Future Projects

Ongoing projects to expand this homelab’s capabilities include:

- **Automation with Ansible**: To streamline configuration management and deployments.
- **Advanced SIEM Customizations**: Enhancing Splunk dashboards and custom log parsing.
- **Backup and Disaster Recovery**: Refining the DR strategy and adding cloud backups.
- **Containerization of Additional Services**: Exploring Kubernetes or Docker Swarm for orchestrating container workloads.

➡️ [See the Future Projects](future-projects.md)

---

Thank you for visiting the cwsecur1ty Documentation Hub. Dive into each section to see the full setup and configuration details of my homelab!
