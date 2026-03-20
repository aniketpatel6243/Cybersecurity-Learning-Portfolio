# Hey, I'm Aniket Patel 👋

I'm a Masters in Information Systems Management student who got genuinely obsessed with cybersecurity. Instead of just studying theory, I started building things — home labs, detection tools, vulnerable apps — anything that helped me understand how attacks actually work and how to stop them.

This is where I document everything I build.

I'm looking for opportunities in **SOC Analysis**, **Security Analysis**, or anything in the **Blue Team / Information Security** space.



## Projects

### 🔴 Wazuh SIEM Home Lab
This is my biggest project so far. I set up a full SIEM using Wazuh on a home lab with two VMs — one running the Wazuh server and one running Kali Linux as both the monitored endpoint and the attack machine.

I didn't just install it and take a screenshot. I wrote custom detection rules from scratch, simulated real attacks like SSH brute force and file tampering, and watched Wazuh catch them in real time. Honestly one of the most satisfying things I've built.

**What I used:** Wazuh 4.7.5 · Kali Linux · Ubuntu 22.04 · VirtualBox · Hydra · MITRE ATT&CK  
📁 [`wazuh-siem-homelab/`](Wazuh-SIEM-labs/)



### 🔴 Web Vulnerability Scanner *(coming soon)*
Building a Python tool to scan web apps for XSS, missing security headers, and directory traversal. Wanted to understand how tools like Burp Suite work under the hood.

**What I'm using:** Python · Requests · OWASP Top 10  
📁 `web-vulnerability-scanner/`



### 🔴 SQL Injection Lab *(coming soon)*
Building a deliberately vulnerable Flask app and a detection script. The goal is to understand SQLi from both sides — how it's exploited and how to defend against it.

**What I'm using:** Python · Flask · SQLite · Web Security  
📁 `sql-injection-lab/`



### 🔴 File Integrity Monitoring Tool *(coming soon)*
A lightweight Python tool that watches critical system files and alerts when something changes. Built after working with Wazuh's FIM module and wanting to understand how it works at a lower level.

**What I'm using:** Python · Linux · File Monitoring  
📁 `file-integrity-monitoring/`


## Things I'm comfortable with

- Setting up and configuring SIEM tools (Wazuh)
- Writing custom detection rules and mapping them to MITRE ATT&CK
- Simulating attacks in a safe lab environment
- Python scripting for security automation
- Linux administration (Ubuntu, Kali)
- Reading and triaging security alerts



## Currently

- 📚 Finishing my Masters in Information Systems Management
- 🔨 Building more projects and adding them here
- 📖 Working towards CompTIA Security+



## Let's connect

- 💼 [LinkedIn](#)
  



*Everything here is built in a home lab for learning purposes. All attacks are performed on systems I own and control.*
