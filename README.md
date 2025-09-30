## 🔐 SIEM Implementation: Wazuh + Suricata

A comprehensive guide demonstrating the deployment and configuration of Wazuh SIEM with Suricata IDS for centralized security monitoring.
This project covers installation, multi-platform agent management (Ubuntu & Windows), and use cases including:

- File Integrity Monitoring (FIM)
- Network Intrusion Detection (Suricata)
- Vulnerability Detection
- Malicious Command Auditing (Auditd)
- SSH Brute Force Protection
- Malware Detection via VirusTotal Integration

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

