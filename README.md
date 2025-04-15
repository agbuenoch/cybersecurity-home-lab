# cybersecurity-home-lab

This project documents the step-by-step process of setting up a **cybersecurity home lab** using **VMware Workstation Pro**, with a detailed guide on downloading and installing Kali-Linux "pre-built image", Ubuntu server "installer image" and VMware Workstation Pro virtualization tool. With these tools, you can simulate attacks using the Kali Linux VM and perform log analysis and monitoring on the Ubuntu server.

# 🛡️ Cybersecurity Home Lab: Kali Linux & Ubuntu Server on VMware Workstation Pro

- 🔍 **Kali Linux (Pre-Built Image)** – for penetration testing and vulnerability scanning  
- 🖥️ **Ubuntu Server (Installer Image)** – as a base for detection tools like Wazuh, ELK, and Splunk  

> 🎯 This lab supports my learning journey into cyber defense, SOC operations, and blue team security analysis.

## 📁 Project Overview

| Component          | Purpose                                                   |
|--------------------|-----------------------------------------------------------|
| VMware Workstation | Virtualization platform                                   |
| Kali Linux         | Offensive security and pentesting                         |
| Ubuntu Server      | Server OS for SIEM and log analysis tools                 |
| Wazuh/Splunk/ELK   | (Coming soon) For real-time log analysis and threat detection |

## 🧰 Tools & Technologies

- VMware Workstation Pro
- Kali Linux (OVA - Pre-Built Image)
- Ubuntu Server 22.04 LTS (Installer ISO)
- CLI Tools (Netplan, `ping`, `ip`, `apt`, etc.)

## 📥 Installation Steps

### 1️⃣ Kali Linux (Pre-Built Image)
- ✅ Downloaded `.ova` file from [Kali Linux Official Site](https://www.kali.org/get-kali/#kali-virtual-machines)
- ✅ Imported into VMware Workstation Pro
- ✅ Verified network, updated system packages

### 2️⃣ Ubuntu Server (Installer Image)
- ✅ Downloaded ISO from [Ubuntu Server Official Site](https://ubuntu.com/download/server)
- ✅ Created new VM in VMware with the ISO mounted
- ✅ Completed guided installation (no desktop environment)
- ✅ Applied basic security hardening (user creation, firewall setup)

## 🔐 Post-Install Hardening (Ubuntu Server)
- Disabled root SSH login
- Created non-root sudo user
- Enabled UFW firewall
- Configured automatic security updates
- Installed essential tools (curl, net-tools, fail2ban, etc.)

## 🚀 What's Next

- ✅ Install and configure **Wazuh Manager**  
- 🔜 Connect AWS and host logs for centralized analysis  
- 🔜 Setup Splunk or ELK for SIEM capabilities  
- 🔜 Run web app attack simulations using DVWA & OWASP Juice Shop  

## 🎯 Learning Goals
- Build and operate a self-hosted, isolated cybersecurity lab  
- Learn how to install and secure Linux servers  
- Simulate attack and detection scenarios  
- Practice log analysis and SIEM setup  

## 👨‍💻 Author
Agbu, Enoch Amachundi  
[🔗 LinkedIn](https://www.linkedin.com/in/agbuenoch)   

## 🏷️ Tags
#CyberSecurity #HomeLab #BlueTeam #KaliLinux #UbuntuServer #VMware #SOCAnalyst #InfoSec #SIEM #HandsOnCybersecurity
