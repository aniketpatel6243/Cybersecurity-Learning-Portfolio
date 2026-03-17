# Wazuh SIEM Home Lab

A hands-on cybersecurity project where I deployed Wazuh SIEM in a virtualized environment, connected a Kali Linux agent, wrote custom detection rules, and simulated real attacks to validate detection.

**Author:** Aniket Patel  
**Duration:** Self-paced home lab  
**Stack:** Wazuh 4.7.5 · Kali Linux · Ubuntu 22.04 · VirtualBox · Hydra

---

## What I Built

Two VMs connected on a Host-Only network:
- **Wazuh Server** (Ubuntu 22.04) — runs the SIEM manager, indexer, and dashboard
- **Kali Linux** — acts as both the monitored endpoint (agent) and the attacker

---

## Custom Detection Rules

I wrote 3 custom XML rules in `/var/ossec/etc/rules/`, each mapped to MITRE ATT&CK:

| Rule ID | Detects | MITRE |
|---|---|---|
| 100001 | SSH Brute Force from same IP | T1110 |
| 100002 | /etc/passwd file modification | T1078 |
| 100003 | Multiple sudo executions | T1548 |

Full rules → [`rules/local_rules.xml`](rules/local_rules.xml)

---

## Attacks Simulated

**1. SSH Brute Force**
```bash
hydra -l root -P /usr/share/wordlists/rockyou.txt 192.168.x.x ssh -t 4
```
Rule 100001 fired after 5 failed attempts from same IP.

**2. File Integrity Monitoring**
```bash
sudo touch /etc/passwd
```
Rule 100002 fired detecting critical file access.

**3. Privilege Escalation**
```bash
sudo cat /etc/shadow
sudo cat /etc/passwd
sudo cat /etc/hostname
```
Rule 100003 fired detecting repeated sudo usage.

---

## Screenshots

All screenshots are in the [`screenshots/`](screenshots/) folder showing attack simulation and alert detection on the Wazuh dashboard.

---

## What I Learned

- How SIEM systems collect and correlate logs from multiple endpoints
- Writing custom OSSEC/Wazuh detection rules from scratch
- How attackers perform brute force, FIM bypass, and privilege escalation
- Alert triage and analysis using OpenSearch Dashboard
- MITRE ATT&CK framework mapping for real attack techniques

---

*Built for educational purposes in a controlled home lab environment.*

## Tools & Technologies

![Wazuh](https://img.shields.io/badge/Wazuh-4.7.5-blue)
![Kali Linux](https://img.shields.io/badge/Kali-Linux-557C94)
![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-E95420)
![VirtualBox](https://img.shields.io/badge/VirtualBox-7.x-183A61)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red)

---

## Author

**Aniket Patel**  
Cybersecurity Enthusiast | Fresher  
📧 Connect on [LinkedIn](#https://www.linkedin.com/in/aniket-patel-253820253/)  
🔗 [Portfolio Repository](https://github.com/YourUsername/cybersecurity-learning-portfolio)

---

*This project was built entirely in a home lab environment for educational purposes. All attacks were performed on systems owned and controlled by the author.*
