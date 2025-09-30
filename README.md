# 🔐 SIEM Implementation: Wazuh + Suricata
A comprehensive guide demonstrating Wazuh deployment, configuration, and agent management on Ubuntu and Windows. Includes setup for file integrity monitoring, Suricata IDS, vulnerability detection, malicious command auditing, SSH brute force protection, and VirusTotal integration for malware detection.

---

## 📋 Overview

This project documents the full setup of a **centralized security monitoring infrastructure** using Wazuh and Suricata.
It covers installation, configuration, and security demonstrations across **Ubuntu** and **Windows** systems, integrating multiple tools for **threat detection**, **response**, and **monitoring**.

---

## 🛠️ Technologies Used

* **Wazuh** 4.8.1 → Open-source SIEM & XDR
* **Suricata** → Network Intrusion Detection System
* **Ubuntu 22.04** → Primary OS for Wazuh Manager
* **Windows 10** → Agent deployment & monitoring
* **VirusTotal API** → Malware analysis integration
* **Auditd** → Linux system auditing

---

## 🔧 Implemented Features

### 1. Core Infrastructure

* Wazuh Manager installation on Ubuntu 22.04
* Multi-platform agent deployment (Windows & Ubuntu)
* Dashboard setup and configuration

### 2. Security Monitoring

* **File Integrity Monitoring (FIM)** → Real-time file change alerts
* **Network Intrusion Detection** → Suricata + Emerging Threats rules
* **Vulnerability Detection** → OS vulnerability scans for Ubuntu & Windows
* **Command Monitoring** → Auditd integration for root activity detection

### 3. Threat Protection

* **SSH Brute Force Protection** → Active response rules
* **Malware Detection** → VirusTotal integration for suspicious files
* **Custom Alert Rules** → Tailored detection policies

---

## 📁 Project Structure

```
├── Documentation/        # Detailed implementation report
├── Configurations/       # Sample config files
│   ├── ossec.conf        # Wazuh main configuration
│   ├── suricata.yaml     # Suricata configuration
│   └── audit.rules       # Auditd rules
└── README.md             # Project documentation
```

---

## 🚀 Quick Start

### Prerequisites

* Ubuntu 20.04+ VM (Wazuh Manager)
* Windows VM (Agent)
* Additional Ubuntu VM (Agent)
* Proper network connectivity between systems

### Installation

**Wazuh Manager Setup:**

```bash
curl -sO https://packages.wazuh.com/4.8/wazuh-install.sh
sudo bash ./wazuh-install.sh -a
```

**Agent Deployment:**

* Install Wazuh agents on **Windows** and **Ubuntu** hosts
* Configure agent communication with the Wazuh Manager

---

## 📊 Key Demonstrations

* Real-time event monitoring in Wazuh dashboard
* **Nmap scan detection** via Suricata
* File Integrity alerts for unauthorized changes
* OS vulnerability assessment & reporting
* Brute-force SSH detection with automated blocking
* Malware detection using VirusTotal API

---

## 🔍 Use Cases

* **File Integrity Monitoring** → Prevent data tampering
* **Network Security** → Detect scans & intrusion attempts
* **System Hardening** → Identify vulnerabilities & compliance issues
* **Incident Response** → Real-time alerts & active defense
* **Threat Intelligence** → Integration with external feeds

---

## 📈 Results

The implementation demonstrates:
✔ Centralized monitoring across Linux & Windows systems
✔ Effective detection of common attack vectors
✔ Automated threat response mechanisms
✔ Integrated vulnerability management
✔ Alignment with industry-standard security tools

---

## 📚 References

* [Wazuh Documentation](https://documentation.wazuh.com/)
* [Suricata Documentation](https://suricata.io/documentation/)
* [Emerging Threats Ruleset](https://rules.emergingthreats.net/)

---

> ⚠️ **Disclaimer**: This project is built for **educational and demonstration purposes** only, within a controlled lab environment.

