# SSH Brute-Force Attack Simulation & Alert Monitoring

This document demonstrates simulated attack activity against the Wazuh environment using Hydra to test real-time alert detection and security event logging on the dashboard.

---

### Step 1: Executing SSH Brute-Force Attack with Hydra
<img width="1118" height="208" alt="triggering an alert" src="https://github.com/user-attachments/assets/25aed553-54f1-467c-89e8-27ccf4864afc" />

**Description:** Executed an automated SSH password brute-force attack from the Kali Linux host against the target (`192.168.29.99`) using `hydra` with the `unix_passwords.txt` wordlist for user `wazuh-user`.

---

### Step 2: Monitoring Security Alerts on Wazuh Dashboard
<img width="1177" height="626" alt="dashboard event analysis" src="https://github.com/user-attachments/assets/155929ea-7a5f-4b67-921b-b3eb3897f04b" />

**Description:** Monitored the real-time security impact in the Wazuh **Threat Hunting** dashboard. The manager successfully detected **3,235 Authentication Failures**, mapping the activity directly to MITRE ATT&CK techniques such as **Password Guessing** and **Brute Force**.
