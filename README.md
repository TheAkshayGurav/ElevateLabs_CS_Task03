# ElevateLabs_CS_Task03
Perform a Basic Vulnerability Scan on Your PC (Tenable Nessus Essentials)
# 🔎 Basic Vulnerability Scan with Nessus Essentials (Kali Linux)

## 📌 Task Overview
This project demonstrates how to perform a **basic vulnerability scan** on a local machine using **Nessus Essentials** in **Kali Linux**.  
The goal is to gain introductory experience with vulnerability assessment and understand common risks present on a PC.

- **Tool Used:** Nessus Essentials (Free edition by Tenable)  
- **Target:** Localhost (`127.0.0.1`) on Kali Linux  
- **Scan Type:** Basic Network Scan  
- **Deliverables:** Vulnerability scan report, screenshots, remediation notes, and documentation  

---

## ⚙️ Environment
- **OS:** Kali Linux (Rolling, x86_64)  
- **Nessus Version:** [Fill in exact version, e.g., 10.7.5]  
- **Date of Scan:** [YYYY-MM-DD]  
- **Scan Target:** `127.0.0.1`  

---

## 🚀 Step-by-Step Process

### 1. Install Nessus Essentials
```bash
sudo apt update && sudo apt -y upgrade
cd ~/Downloads
sudo dpkg -i Nessus-*.deb
sudo apt-get install -f -y
sudo systemctl start nessusd
sudo systemctl enable nessusd

Access Nessus Web UI
Open browser → https://localhost:8834/
Accept SSL warning (self-signed cert)
Select Nessus Essentials, enter activation code (from Tenable), set admin user/password
Wait for plugin feed to sync (first run may take several minutes)

Create and Launch Scan
Navigate → Scans → New Scan → Basic Network Scan
Name: Localhost - Basic Scan
Target: 127.0.0.1
Save and Launch
Scan takes ~30–60 minutes

xport and Document Results
After completion, export results (PDF/HTML/CSV)
Save reports under reports/ folder
Take screenshots of:
Completed scans list
Vulnerability severity chart
Example vulnerability detail view



