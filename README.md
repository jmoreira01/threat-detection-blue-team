[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![CESAE Digital](https://img.shields.io/badge/CESAE-Digital-blue)](https://www.cesae.pt/)

# 🛡️ Threat Detection - Blue Team Portfolio

> **Cybersecurity Projects Collection** | Security Monitoring, Threat Detection & Incident Response

This repository serves as a centralized index for my Blue Team cybersecurity projects developed during the DETECT Cybersecurity Training program at CESAE Digital.

---

## 👤 About Me

**Name:** Jorge Moreira  
**Program:** DETECT - Cybersecurity Training  
**Institution:** CESAE Digital  
**Focus Areas:** Blue Team Operations, SIEM Implementation, Threat Detection, Incident Response

**Specializations:**
- 🔍 Security Information and Event Management (SIEM)
- 🛡️ File Integrity Monitoring (FIM)
- 🦠 Malware Detection & Analysis (YARA)
- 🔍 Network Intrusion Detection (Suricata)
- ⚡ Automated Threat Response
- 🎯 MITRE ATT&CK Framework Mapping
- 🔐 Windows & Linux Security Hardening

---

## 📚 Projects Overview

### 🔥 Featured Projects

#### 1. 🏢 [SIEM LAB Implementation](https://github.com/jmoreira01/siem-lab-project)

**Enterprise SIEM Deployment with Wazuh**

Complete security monitoring solution for enterprise infrastructure with real-time threat detection and automated response capabilities.

**Key Features:**
- ✅ Wazuh SIEM (Docker deployment)
- ✅ Multi-platform agents (Windows + Linux)
- ✅ File Integrity Monitoring with real-time alerts
- ✅ YARA malware detection engine
- ✅ Automated IP blocking (Active Response)
- ✅ MITRE ATT&CK framework mapping

**Technologies:** Wazuh v4.14.2 | Docker | YARA v4.5.5 | PowerShell | Bash  
**Detection Rate:** 100% across all simulated attacks  
**Response Time:** <15 seconds average

**Attack Scenarios Tested:**
- SSH/RDP Brute Force (T1110.001)
- SQL Injection (T1190)
- Malware Upload (T1204.002)
- Malicious IP Access (T1071)

[📖 View Project →](https://github.com/jmoreira01/siem-lab-project)

---

#### 2. 📚 [Wazuh Configuration Guides & Best Practices](https://github.com/jmoreira01/WAZUH_YARA_Complete_Configuration)

**Comprehensive technical documentation and configuration templates**

A collection of curated Wazuh configurations, troubleshooting guides, and best practices developed through hands-on implementation experience.

**Includes:**
- 📝 Complete configuration templates (Server + Agents)
- 🔧 YARA integration guides (Windows + Linux)
- 🚨 Custom rules library for threat detection
- 🎯 Active Response automation scripts
- 🐛 Troubleshooting methodologies
- ✅ Configuration checklists

**Coverage:**
- Server configuration (Manager, Indexer, Dashboard)
- Windows Agent setup and hardening
- Linux Agent deployment
- FIM advanced configurations
- CDB lists for IP reputation
- Decoder and rule customization

**Languages:** English + Portuguese  
**Format:** Markdown documentation with code examples

[📖 View Project →](https://github.com/jmoreira01/WAZUH_YARA_Complete_Configuration)

---

#### 3. 🔍 [Suricata IDS Integration with Wazuh](https://github.com/jmoreira01/suricata-ids-integration)

**Network Intrusion Detection with Suricata integrated into Wazuh SIEM**

Implementation of a Network Intrusion Detection System (NIDS) using Suricata, fully integrated with Wazuh for centralized monitoring, alert correlation, and automated threat response.

**Key Features:**
- ✅ Suricata 8.0.3 NIDS with Emerging Threats ruleset
- ✅ Real-time network traffic analysis and alerting
- ✅ Wazuh SIEM integration for centralized alert correlation
- ✅ Active Response — automated IP blocking on NMAP detection
- ✅ Multi-vector detection combining NIDS + HIDS
- ✅ Comprehensive troubleshooting documentation

**Technologies:** Suricata 8.0.3 | Wazuh SIEM | Ubuntu 22.04 | Kali Linux | NMAP | GoldenEye

**Attack Scenarios Tested:**
- NMAP Vulnerability Scanning (T1595.002) — 3,539 alerts generated
- GoldenEye HTTP DoS (T1499) — Agent queue saturation detected
- Automated NMAP blocking via Active Response (<5 sec response)

**Detection Highlights:**
- Suricata ET SCAN rules detected NMAP scripting engine
- Wazuh correlated network alerts with application-layer errors
- Indirect DoS indicators identified through agent queue monitoring

[📖 View Project →](https://github.com/jmoreira01/suricata-ids-integration)

---

## 🛠️ Technical Stack

### Operating Systems

- 🪟 **Windows:** 10, 11, Server 2019/2022
- 🐧 **Linux:** Debian 13, Ubuntu 22.04, Kali Linux
- 🐳 **Virtualization:** VirtualBox, VMware, Docker

### Programming & Scripting

- **Bash** - Automation scripts, YARA integration
- **PowerShell** - Windows security automation
- **Python** - Custom security tools, data analysis
- **XML** - Wazuh rules and decoders

---

## 📊 Skills Demonstrated

### Blue Team Competencies

✅ **Security Monitoring**
- Real-time log analysis and correlation
- Event triage and prioritization
- Alert tuning and false positive reduction

✅ **Threat Detection**
- Signature-based detection (YARA, Suricata)
- Anomaly detection (FIM)
- Network intrusion detection (NIDS)
- Behavioral analysis
- IOC identification

✅ **Incident Response**
- Automated response mechanisms
- IP blocking and containment
- Security event investigation
- Post-incident documentation

✅ **Security Architecture**
- SIEM deployment and configuration
- IDS/NIDS integration
- Multi-platform agent management
- Network segmentation awareness
- Defense in depth strategies

✅ **Documentation**
- Technical writing and documentation
- Configuration management
- Standard Operating Procedures (SOPs)
- Knowledge base creation

---

## 🎯 MITRE ATT&CK Coverage

### Tactics & Techniques Addressed

| Tactic | Technique | ID | Implementation |
|--------|-----------|-----|----------------|
| **Reconnaissance** | Active Scanning: Vulnerability Scanning | T1595.002 | Suricata NMAP detection + Active Response |
| **Reconnaissance** | Active Scanning: Scanning IP Blocks | T1595.001 | Suricata network monitoring |
| **Credential Access** | Brute Force: Password Guessing | T1110.001 | SSH/RDP monitoring + blocking |
| **Initial Access** | Exploit Public-Facing App | T1190 | Apache log analysis, SQL injection detection |
| **Execution** | User Execution: Malicious File | T1204.002 | YARA malware scanning |
| **Defense Evasion** | Indicator Removal | T1070 | File Integrity Monitoring |
| **Command & Control** | Application Layer Protocol | T1071 | IP reputation blocking |
| **Persistence** | Create Account | T1136 | Account creation monitoring |
| **Discovery** | System Information Discovery | T1082 | System log analysis |
| **Impact** | Endpoint Denial of Service | T1499 | Suricata + agent queue monitoring |
| **Impact** | Network Denial of Service | T1498 | Suricata traffic anomaly detection |

---

## 📈 Project Statistics

### Technology Breakdown

```
Wazuh Configuration    ████████████████████░  95%
YARA Integration       ██████████████████░░  90%
Suricata IDS           ████████████████████░  95%
Active Response        █████████████████░░░  88%
FIM Implementation     ████████████████████░  95%
Docker Deployment      ██████████████░░░░░░  75%
Custom Rule Writing    ████████████████░░░░  85%
Documentation          ████████████████████░  98%
```

## 🎓 Learning Journey

### DETECT Cybersecurity Training Program

**Institution:** CESAE Digital  
**Duration:** 2025-2026  
**Focus:** Practical Blue Team Operations

**Completed Modules:**
- ✅ SIEM Implementation & Management
- ✅ Threat Detection Methodologies
- ✅ Incident Response Procedures
- ✅ Security Monitoring & Logging
- ✅ Malware Analysis Fundamentals
- ✅ Network Security Monitoring
- ✅ Network Intrusion Detection (Suricata)

**Key Achievements:**
- 100% detection rate on all security labs
- Developed 15+ custom Wazuh detection rules
- Implemented automated response for 5+ attack types
- Integrated Suricata NIDS with Wazuh for multi-layer detection
- Completed comprehensive MITRE ATT&CK mapping
- Created bilingual technical documentation


## 🔗 Links & Resources

### My Projects

- 🏢 [SIEM LAB Implementation](https://github.com/jmoreira01/siem-lab-project)
- 📚 [Wazuh Configuration Guides & Best Practices](https://github.com/jmoreira01/WAZUH_YARA_Complete_Configuration)
- 🔍 [Suricata IDS Integration with Wazuh](https://github.com/jmoreira01/suricata-ids-integration)

### Professional Profiles

- 💼 [LinkedIn](https://www.linkedin.com/in/jormoreira/)
- 💼 [Portfolio](https://jorge-moreira-portfolio.vercel.app/)


### External Resources

**Official Documentation:**
- [Wazuh Documentation](https://documentation.wazuh.com)
- [Suricata Documentation](https://docs.suricata.io/)
- [MITRE ATT&CK](https://attack.mitre.org)
- [YARA Documentation](https://yara.readthedocs.io)


## 📄 License

All projects in this portfolio are licensed under the MIT License unless otherwise specified.

See individual project repositories for specific licensing information.
