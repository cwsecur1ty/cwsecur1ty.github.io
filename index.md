---
layout: default
title: "Home"
---

<!-- LinkedIn logo and link at the top -->
<div style="text-align: center; margin-bottom: 20px;">
  <a href="https://www.linkedin.com/in/cameron-ws/" target="_blank" aria-label="LinkedIn">
    <img src="https://cdn-icons-png.flaticon.com/512/61/61109.png" alt="LinkedIn" style="width: 30px; height: 30px;"/>
  </a>
</div>

# Comprehensive Guide to My Homelab Infrastructure and Security Projects

This hub documents the design, setup, and ongoing projects of my homelab & security projects. Here, you’ll find resources on each part of my Proxmox-based homelab, covering network configuration, services, monitoring, and future project plans.

---

## 📖 Table of Contents

1. [Overview](#overview)
2. [Homelab Setup](#Homelab-Setup)
3. [Installed Services](#installed-services)
4. [Server Architecture](#server-architecture)
5. [Security and Monitoring](#security-and-monitoring)
6. [Future Projects](#future-projects)

---

## Overview

My home lab is built on Proxmox and is designed to host various services for IT support and cybersecurity learning, experimentation, and documentation. This documentation hub will also feature network diagrams, architecture overviews, and configuration steps for anyone interested in replicating or learning from this setup.

---

## 🖧 Homelab Setup

The lab setup involves a segmented architecture allowing isolated environments for different services, improving both organisation and security. Key elements include:

- **Proxmox**: Proxmox VE is used to manage my VMs, containers and storage.
- **Virtual Machines**: Virtual environments where services are running (e.g., media, testing & security).
  
➡️ [Learn more about the Homelab Setup](homelab_setup.md)

---

## ⚙️ Installed Services

My homelab hosts several services for IT and cybersecurity experimentation:

- **Proxmox Virtualization**: Foundation of the homelab, providing resource allocation and VM management.
- **SIEM Tools (Splunk)**: Set up for log aggregation, analysis, and security monitoring with a web interface.
- **Pihole**: Network-level ad blocker for network security and monitoring.
- **Docker and Containers**: Hosting various services in isolated environments.
  
➡️ [Explore the Installed Services](services.md)

---

## 🖥️ Server Architecture

The physical and virtual architecture includes several components designed to optimize performance, scalability, and redundancy. 

- **Proxmox Hosts**: Details on virtualized servers, including memory, CPU, and storage allocation.
- **Storage Solutions**: _Need to acquire more drives for disk failover._
- **Backups and Snapshots**: _Need to acquire a backup server for redundancy._

➡️ [View the Server Architecture](architecture.md)

---

## 🔒 Security and Monitoring

Security is a priority for the homelab, with multiple tools and processes in place for monitoring and threat detection.

- **Firewall and Intrusion Detection**: Configuration of firewalls and IDS/IPS tools.
- **SIEM Analysis**: Using Splunk for real-time log analysis.
- **Network Monitoring**: _Need to implement Zabbix or Nagios to keep track of network and server health._

➡️ [Dive into Security and Monitoring](security.md)

---

## 🚀 Future Projects

Ongoing projects to expand this homelab’s capabilities include:

- **Advanced SIEM Customizations**: Enhancing Splunk dashboards and custom log parsing.
- **Backup and Disaster Recovery**: Refining the DR strategy and adding cloud backups.
- **Containerization of Additional Services**: Exploring Kubernetes or Docker Swarm for orchestrating container workloads.

➡️ [See the Future Projects](future-projects.md)

---

Thank you for visiting.

- Cameron
