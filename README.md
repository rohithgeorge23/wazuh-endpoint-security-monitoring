# 🛡️ Endpoint Security Monitoring via Wazuh SIEM

A hands-on cybersecurity lab implementing a **Wazuh SIEM** architecture inside Oracle VirtualBox. This project covers end-to-end setup, endpoint integration with Kali Linux, automated attack simulation, and real-time alert triage.

---

## 📁 Project Documentation

* 🛠️ **[Installation & VirtualBox Setup](./Wazuh%20Setup%20%26%20Installation%20Process.md)**
* 🔑 **[Wazuh Server Login & Console Access](./Wazuh%20Server%20Login%20Process.md)**
* 💻 **[Wazuh Agent Deployment on Kali Linux](./Wazuh%20Agent%20Deployment%20Process.md)**
* 🚨 **[Attack Simulation & Alert Monitoring](./Alert%20Testing%20%26%20Security%20Monitoring.md)**

---

## 🔑 Key Findings

* **Finding 1:** Wazuh detected the attack in real time by automatically triggering predefined security rules after multiple failed authentication attempts.
* **Finding 2:** The alert system accurately identified the source IP and mapped the activity to relevant MITRE ATT&CK techniques (Password Guessing & Brute Force).
* **Finding 3:** Wazuh assigned an appropriate severity level, enabling clear alert prioritization and effective risk-based classification.

---

## 🎯 Final Conclusion

This project successfully implemented a **Wazuh SIEM environment** to monitor and secure a virtual infrastructure. By integrating a Kali Linux agent and simulating attacks, the system effectively detected real-time threats such as SSH brute-force attempts. 

The results demonstrate Wazuh’s strength in **centralized log management**, **accurate alerting**, and **proper threat prioritization**. Overall, this project emphasizes the critical importance of continuous monitoring and automated security controls in modern cybersecurity operations.
