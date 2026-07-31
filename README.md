# 🛡️ Endpoint Security Monitoring via Wazuh SIEM

A hands-on cybersecurity lab implementing a **Wazuh SIEM** architecture inside Oracle VirtualBox. This project covers end-to-end setup, endpoint integration with Kali Linux, automated attack simulation, and real-time alert triage.

---

## 🚀 Project Overview

This project demonstrates the end-to-end deployment, configuration, and security monitoring capabilities of the **Wazuh Open Source Security Platform (v4.14.2)** in a virtualized lab environment. 

The primary objective was to establish a fully functional SIEM environment to detect real-time brute-force attacks on SSH services and observe log ingestion, correlation, and MITRE ATT&CK mapping via the Wazuh Dashboard.

---

## 📁 Project Documentation

* 🛠️ **[Installation & VirtualBox Setup](./Wazuh%20Setup%20%26%20Installation%20Process.md)**
* 🔑 **[Wazuh Server Login & Console Access](./Login%20Process%20of%20Wazuh%20Server.md)**
* 💻 **[Wazuh Agent Deployment on Kali Linux](./Wazuh%20Agent%20Deployment%20Process.md)**
* 🚨 **[Attack Simulation & Alert Monitoring](./Alert%20Testing%20%26%20Security%20Monitoring.md)**

---


### 🧱 Environment Architecture

| Component | Details |
| :--- | :--- |
| **SIEM Server** | **Wazuh v4.14.2** (Amazon Linux 2023 OVA) on Oracle VirtualBox |
| **Monitored Endpoint** | **Kali GNU/Linux 2025.2** with **Wazuh Agent v4.14.2** |
| **Attack/Testing Machine** | **Kali Linux** (same host used for both agent + attack simulation) |
| **Virtualization Platform** | **Oracle VirtualBox** |

### Network Layout:

* **Wazuh Manager:** `192.168.29.99`
* **Kali Agent (monitored endpoint):** `192.168.29.173`

---

## 📦 Prerequisites

### System Requirements

* **Oracle VirtualBox:** Version 6.1 or higher
* **Host Machine RAM:** Minimum 8GB (16GB+ recommended)
* **Disk Space:** 50GB free minimum
* **Network:** Internet connectivity for package downloads and agent communication
* **Permissions:** Administrator / root access on host machine and virtual instances

### Required Downloads

1. **Wazuh OVA Image (v4.14.2)** — [Official Wazuh Documentation](https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html)
2. **Oracle VirtualBox** — [VirtualBox Official Download Page](https://www.virtualbox.org/)
3. **Kali Linux VM / ISO** — [Kali Linux Downloads Page](https://www.kali.org/get-kali/)

---

## 🛠️ Technologies & Tools

| Technology | Version | Purpose |
| :--- | :--- | :--- |
| **Wazuh** | **4.14.2** | Open-source SIEM & threat detection |
| **Wazuh Agent** | **4.14.2** | Endpoint monitoring and log collection |
| **Kali Linux** | **2025.2** | Monitored endpoint + attack simulation |
| **Oracle VirtualBox** | **7.0+** | Virtualization and VM management |
| **Amazon Linux** | **2023** | Wazuh server base OS |
| **Hydra** | **9.5** | SSH brute-force attack simulation |

---

## 🔑 Key Findings

* **Finding 1:** Wazuh detected the attack in real time by automatically triggering predefined security rules after multiple failed authentication attempts.
  
* **Finding 2:** The alert system accurately identified the source IP and mapped the activity to relevant MITRE ATT&CK techniques (Password Guessing & Brute Force).
  
* **Finding 3:** Wazuh assigned an appropriate severity level, enabling clear alert prioritization and effective risk-based classification.

---


## 🎯 Final Conclusion

This project successfully implemented a **Wazuh SIEM environment** to monitor and secure a virtual infrastructure. By integrating a Kali Linux agent and simulating attacks, the system effectively detected real-time threats such as SSH brute-force attempts. 

The results demonstrate Wazuh’s strength in **centralized log management**, **accurate alerting**, and **proper threat prioritization**. Overall, this project emphasizes the critical importance of continuous monitoring and automated security controls in modern cybersecurity operations.

---

## 📚 References & Resources

* [Wazuh Official Documentation](https://documentation.wazuh.com/)
* [Hydra — THC-Hydra GitHub](https://github.com/vanhauser-thc/thc-hydra)
* [MITRE ATT&CK Framework](https://attack.mitre.org/)

---

## 👤 Author & Contact

**Rohith George**

* **LinkedIn:** https://www.linkedin.com/in/rohithgeorge-bsc?utm_source=share_via&utm_content=profile&utm_medium=member_android

