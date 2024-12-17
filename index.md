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

# Cameron's Documentation Hub

Design, setup, and ongoing projects of my homelab & security projects.

---

## Contents

1. [Overview](#overview)
2. [Homelab Setup](#🖧-Homelab)
3. [AWS Projects](#aws)
4. [Coding/Dev Project Work](#Coding/Dev-Project-Work)
5. [Server Architecture](#server-architecture)
6. [Security and Monitoring](#security-and-monitoring)
7. [Future Projects](#future-projects)

---

## Overview

This page acts as an index for all of my project work across AWS, Development and Labbing.

---

## 🖧 Homelab

The lab setup involves a segmented architecture allowing isolated environments for different services, improving both organisation and security. Key elements include:

- **Proxmox**: Proxmox VE is used to manage my VMs, containers and storage.
- **Virtual Machines**: Virtual environments where services are running (e.g., media, testing & security).

---

## AWS

Collection of AWS projects; Cloud solutions, security automation, and scalable architectures. Each project is designed to showcase practical skills with AWS services.

- [Website Hosting on S3 with CloudFront](aws-s3-website.md) (A secure, cost-effective static website hosted on S3 with global delivery via CloudFront.)
  

---

## ⚙️ Coding/Dev Project Work

My featured projects are:

(All projects are a consistent work in progress to keep them updated with standards and patches)

- **[PowerShell Scripts](https://github.com/cwsecur1ty/PowerShell-Scripts)**: PowerShell scripts to remediate and push fixes through Intune.
- **[URL Hunter](https://github.com/cwsecur1ty/URLHunter)**: A fast and efficient web directory brute-forcer/scanner. It is designed to uncover hidden directories and files on web servers by using a wordlist.
- **[Port Hunter](https://github.com/cwsecur1ty/PortFinder)** Python tool for scanning ports on one or more target IP addresses or URLs. It supports scanning a range of ports, resolving hostnames to IP addresses, and saving scan results to a file.
- **[Sentinel C2](https://github.com/cwsecur1ty/SentinelC2)** This project aimed to better my understanding of Command and Control (C2) servers and expand my defensive skills against such threats.
- **[Debian/Linux Hardener Toolkit/Automation](https://github.com/cwsecur1ty/Debian-Hardener-Toolkit)**: A toolkit for automating Linux security hardening and compliance auditing
- **SIEM Tools (Splunk)**: Set up for log aggregation, analysis, and security monitoring with a web interface on my home lab.
- **Pihole**: Network-level ad blocker for network security and monitoring on my home network, hosted on my ProxMox machine.
  
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
