# SIEM-LAB-Project
Security Information and Event Management (SIEM) setup with Wazuh, Windows agent, and Suricata IDS.

# Wazuh SIEM Lab Project

This project documents the setup of a **Wazuh-based SIEM lab** with Windows endpoints, Suricata network monitoring, and a centralized Wazuh server.  
The lab was built step by step, with each stage documented in detail.
---

## 📌 Project Overview

- **Manager VM (Ubuntu)** → Runs Wazuh Manager, Indexer, Dashboard.  
- **Windows VM** → Wazuh agent installed; collects event logs, Sysmon logs, firewall logs, Suricata logs.  
- **Kali VM (optional)** → Used for attack simulation.  
- **Suricata (Windows)** → IDS/IPS log source.  

---

## 📂 Documentation Steps

1. **[Step 1 - VM Setup](step1_vm_setup.md)**  
   - VirtualBox network setup  
   - Creating Ubuntu server, Windows client VMs  

2. **[Step 2 - Wazuh Implementation](step2_wazuh_implementation.md)**  
   - Installing Wazuh manager, indexer, dashboard  
   - Initial configuration  

3. **[Step 3 - Agent Deployment](step3_agent_deployment.md)**  
   - Installing Wazuh agent on Windows  
   - Connecting agent to manager  

4. **[Step 4 - Log Collection](step4_log_collection.md)**  
   - Collecting Windows event logs, firewall logs, Sysmon logs  
   - File Integrity Monitoring (FIM)  

5. **[Step 5 - Suricata Integration](step5_suricata_integration.md)**  
   - Installing Suricata on Windows  
   - Forwarding Suricata alerts to Wazuh  

6. **[Step 6 - Custom Rules](step6_custom_rules.md)**  
   - Writing Wazuh rules for failed logins, brute force, FIM changes, and Suricata alerts  

7. **[Step 7 - Validation & Testing](step7_validation.md)**  
   - Triggering test events (failed logins, file changes, nmap scans)  
   - Verifying alerts in Wazuh  

8. **[Step 8 - Dashboards & Reporting](step8_dashboards_reporting.md)**  
   - Building saved searches and visualizations  
   - Creating dashboards for Windows, Suricata, and FIM alerts  
   - Exporting PDF reports  

---

## 🚀 Current State

- ✅ Wazuh environment deployed  
- ✅ Windows agent connected  
- ✅ Suricata integrated  
- ✅ Custom rules tested  
- ✅ Dashboards & PDF reporting  

---

## 📖 References

- [Wazuh Documentation](https://documentation.wazuh.com)  
- [Suricata Documentation](https://suricata.io/)  

---
