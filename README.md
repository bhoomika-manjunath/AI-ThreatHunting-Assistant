# 🛡️ HuntForge — AI Threat Hunting Assistant & SOC Intelligence Platform

[![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-v14.1-blue.svg)](https://attack.mitre.org/)
[![Sigma](https://img.shields.io/badge/Sigma-Detection%20Rules-teal.svg)](https://github.com/SigmaHQ/sigma)
[![NIST CSF](https://img.shields.io/badge/NIST-CSF%202.0-green.svg)](https://csrc.nist.gov/)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-Vercel-000000.svg?logo=vercel&logoColor=white)](https://ai-threat-hunting-assistant.vercel.app)
[![License](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)

🌐 **Live Platform**: [ai-threat-hunting-assistant.vercel.app](https://ai-threat-hunting-assistant.vercel.app)

> **HuntForge** is an advanced AI-augmented cybersecurity threat hunting and detection engineering platform. It bridges the gap between raw, complex security telemetry and rapid incident response by translating natural language incident descriptions into structured MITRE ATT&CK mappings, production-grade Sigma rules, dynamic Cyber Kill Chain profiles, and automated containment playbooks.

---

## ⚡ Key Capabilities

### 1. 🤖 Autonomous Threat Investigation Studio
- **Natural Language Analysis**: Describe observed suspicious activity, anomalous event logs, or IOCs to get instant tactical breakdown.
- **Pre-Configured Threat Scenarios**: Instant 1-click simulations for:
  - `LockBit 3.0 Ransomware` (VSS shadow copy deletion & mass AES encryption)
  - `Active Directory Pass-the-Hash` (LSASS dumping & PsExec lateral movement)
  - `AWS IAM Privilege Escalation` (Unauthorized policy attachment & key generation)
  - `DNS Tunneling Exfiltration` (High-entropy TXT records)
  - `Cobalt Strike C2 Beaconing` (Malleable HTTPS jitter beacons)
- **Dual AI Engine**: Zero-dependency offline cybersecurity intelligence synthesizer + native Anthropic Claude 3.7 API integration.

### 2. 📊 Live SOC Telemetry Dashboard
- Real-time KPI metrics: **Active Threat Hunts**, **Mean Time to Detect (MTTD)**, **Sigma Coverage Index (98.4%)**, and **Attacker Dwell Time Prevented**.
- Interactive **Weekly Threat Velocity & Hunt Volume** chart built with Chart.js.
- Streaming real-time SOC activity feed with severity classification.

### 3. 🎯 Interactive MITRE ATT&CK Matrix Explorer
- Heat matrix covering enterprise tactics: *Initial Access*, *Execution*, *Persistence*, *Credential Access*, *C2*, and *Impact*.
- Clickable technique cards (*T1059.001 PowerShell*, *T1003.001 LSASS Memory*, *T1486 Data Encrypted*, etc.) with direct investigation triggers.

### 4. 📝 Automated Sigma Detection Rule Generator
- Generates production-ready, syntactically validated Sigma YAML rules compatible with Splunk, Microsoft Sentinel, Elastic, and QRadar.
- Integrated 1-click clipboard copy and `.yml` file download.

### 5. 🛡️ NIST-Aligned Containment Playbooks
- Context-aware containment, process isolation, credential revocation, and forensic preservation instructions for SOC Tier 1-3 analysts.

### 6. 📄 Multi-Format Threat Dossier Export
- **Print-ready PDF Threat Dossier** with executive summary, technique breakdown, and remediation steps.
- **Sigma YAML (`.yml`)** file download.

---

## 🏗️ Architecture Pipeline

```
[ Security Telemetry / Natural Language Query ]
                       │
                       ▼
         [ Semantic ATT&CK Mapping Engine ]
   (Tactics, Techniques, Sub-Techniques v14)
                       │
                       ▼
       ┌───────────────┴───────────────┐
       ▼                               ▼
[ Sigma Rule Compiler ]      [ Kill Chain Profiler ]
(Splunk/Sentinel Ready)     (12-Stage Radar Matrix)
       │                               │
       └───────────────┬───────────────┘
                       ▼
     [ NIST Containment Playbook & Threat Dossier ]
```

---

## 🚀 Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/bhoomika-manjunath/AI-ThreatHunting-Assistant.git
   ```
2. Open `index.html` in any modern web browser — no dependencies, node servers, or builds required!

---

## 🔒 Security & Privacy

- All analysis in Smart Demo mode executes entirely in-browser.
- Custom API keys entered in Engine Settings remain in browser session memory and are never persisted to external servers.

---

## 📜 Standards & References

- [MITRE ATT&CK Enterprise Matrix](https://attack.mitre.org/matrices/enterprise/)
- [SigmaHQ Generic Signature Format](https://github.com/SigmaHQ/sigma)
- [NIST Computer Security Incident Handling Guide (SP 800-61 Rev. 2)](https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final)

---

&copy; 2026 Bhoomika Manjunath. Built for CISOs, SOC Analysts, and Threat Detection Engineers.
