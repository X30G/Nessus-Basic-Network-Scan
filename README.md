# 🔍 Nessus Vulnerability Scan on Metasploitable3

This project demonstrates a **basic network vulnerability scan** using **Tenable Nessus 10.9.1** against a vulnerable virtual machine, **Metasploitable3**, as the target. It’s designed to showcase the ability to identify, assess, and report on potential security issues in a controlled lab environment.

## 🎯 Project Purpose

This is a demonstration project for:
- Practicing vulnerability assessment skills.
- Showcasing network scanning using professional-grade tools.
- Sharing a reproducible workflow for cybersecurity learning.

Target audience: **Recruiters**, **home lab enthusiasts**, and the broader **infosec community**.

---

## 🧰 Tools & Environment

| Tool           | Details                                |
|----------------|----------------------------------------|
| Host OS        | Kali Linux (running Nessus)            |
| Target VM      | Metasploitable3                        |
| Scanner        | Tenable Nessus                         |
| Virtualization | VirtualBox                             |
| Network Setup  | Host-only Adapter (`vboxnet0`) + NAT   |

---

## ⚙️ Lab Setup Overview

The lab consists of two VMs running inside **VirtualBox**:

1. **Kali Linux (Nessus Installed)** – the scanner.
2. **Metasploitable3** – the target.

**Networking**:
- **Host-Only Adapter** (`vboxnet0`) for direct communication between VMs.
- **NAT Adapter** for internet access and Nessus plugin updates.

This setup isolates the vulnerable machine from the broader internet while allowing the scanner to reach it locally.

---

## 🚀 Scan Details

- **Nessus Template**: Basic Network Scan
- **Target**: Metasploitable3 local IP (e.g., `192.168.x.x`)
- **Port Range**: `1 - 65535` (full TCP port scan)
- **Authentication**: None (unauthenticated scan)

---

## 📸 Results & Deliverables

Included in this repository:
- 📄 **Scan Report** (PDF) [Nessus Report](./Basic%20Net%20Scan.pdf/)
- 🖼️ **Screenshots** of the Nessus scan process and findings [screenshots](./screenshots/)
- 📝 **Setup notes** for replicating the environment

---

## 🔁 Replication Guide

While this lab uses **VirtualBox**, the scan can be replicated using any virtualization platform that supports custom network adapters.

Ensure your scanner (Kali + Nessus) and target (Metasploitable3) are on the same host-only network.

---

## 🛡️ Disclaimer

This lab is for **educational and demonstration purposes only**. Never run vulnerability scans on systems you do not own or have explicit permission to test.

---
