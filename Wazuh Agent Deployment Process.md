# Wazuh Agent Deployment on Kali Linux Endpoint

This document outlines the complete process of registering, installing, starting, and verifying a Wazuh security agent on a target endpoint (Kali Linux).

---

### Step 1: Initiate Agent Deployment
<img width="1132" height="597" alt="deploy new agent" src="https://github.com/user-attachments/assets/9bd2d6a2-ac08-4e34-8731-0e98f1109d83" />

**Description:** Accessed the main Wazuh Overview dashboard displaying an empty environment with no agents registered, then clicked on the **Deploy new agent** button.

---

### Step 2: Generating Agent Installation Commands
<img width="1187" height="634" alt="agent list" src="https://github.com/user-attachments/assets/075cfcd7-7801-4367-8db8-1ddf96bb3b02" />

**Description:** Configured the deployment wizard parameters for a Linux system to auto-generate the deployment script specifying the manager IP (`192.168.29.99`) and endpoint name (`kali-linux`).

---

### Step 3: Downloading & Installing the Agent Package
<img width="1087" height="415" alt="verify command" src="https://github.com/user-attachments/assets/f5ff9be7-2209-4734-865c-1b795476fd31" />

**Description:** Executed the generated command inside the Kali Linux endpoint terminal to download the `wazuh-agent_4.14.2-1_amd64.deb` package and install it via `dpkg`.

---

### Step 4: Enabling & Starting the Agent Service
<img width="1070" height="174" alt="agent status" src="https://github.com/user-attachments/assets/f7abf78b-6c85-409a-9aec-433d04be78a2" />

**Description:** Reloaded the system daemon, enabled `wazuh-agent` to start on boot, and started the service using `systemctl start wazuh-agent`.

---

### Step 5: Verifying Agent Connection on Manager Dashboard
<img width="1154" height="548" alt="confirm agent connection" src="https://github.com/user-attachments/assets/7a048d92-c35e-4c7b-9342-34a7c2102ba6" />

**Description:** Returned to the Wazuh Web UI **Endpoints** tab to confirm that agent `001` (`kali-linux` @ `192.168.29.173`) was successfully registered with an **Active** status.
