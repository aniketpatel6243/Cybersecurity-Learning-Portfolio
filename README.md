Cybersecurity Home Lab & Portfolio
I'm a Masters in Information Systems Management student who got genuinely obsessed with cybersecurity. Instead of just studying theory, I started building things — home labs, detection tools, SIEM environments — anything that helped me understand how attacks actually work and how to stop them.
This is where I document everything I build.
I'm looking for opportunities in SOC Analysis, Security Analysis, or anything in the Blue Team / Information Security space.

Projects


🔵 Splunk SIEM — SSH Brute Force Investigation
My first deep dive into Splunk as a SIEM platform. I ingested real Zeek network capture logs containing 7,143 SSH connection events and investigated a large-scale brute force attack campaign from start to finish.

I didn't just upload the data and run a default search. I configured custom field extractions using regex to parse the Zeek log format, wrote SPL queries to identify the top attacking IPs, uncovered multiple successful unauthorized SSH logins, built a full SOC analyst dashboard with attack timelines and status breakdowns, and documented everything as a professional incident report.
The critical finding was discovering that multiple source IPs achieved successful SSH logins — a real incident that would trigger immediate response in a production environment.

What I used: Splunk Enterprise · Zeek/Bro Network Logs · SPL · Windows 11 · Field Extractions · Custom Dashboards

🔵 Wazuh SIEM Home Lab
My biggest project so far. I set up a full SIEM using Wazuh on a home lab with two VMs — one running the Wazuh server and one running Kali Linux as both the monitored endpoint and the attack machine.

I didn't just install it and take a screenshot. I wrote custom detection rules from scratch, simulated real attacks like SSH brute force and file tampering, and watched Wazuh catch them in real time. Honestly one of the most satisfying things I've built.

What I used: Wazuh 4.7.5 · Kali Linux · Ubuntu 22.04 · VirtualBox · Hydra · MITRE ATT&CK
📁 wazuh-siem-homelab/(Wazuh-SIEM-labs)


What I'm Comfortable With

Ingesting, parsing and analyzing logs in Splunk using SPL queries
Setting up and configuring SIEM tools (Splunk, Wazuh)
Writing custom detection rules and mapping them to MITRE ATT&CK
Simulating attacks in a safe lab environment and validating detections
Building SOC dashboards for real-time threat visibility
Investigating security incidents — identifying attackers, attack patterns and compromise indicators
Python scripting for security automation
Linux administration (Ubuntu, Kali)
Reading, triaging and documenting security alerts
Writing professional incident reports


Tools and Technologies

CategoryToolsSIEMSplunk Enterprise, WazuhQuery LanguagesSPL (Splunk Processing Language)Network AnalysisZeek/Bro, WiresharkAttack SimulationHydra, Kali LinuxFrameworksMITRE ATT&CKScriptingPythonOperating SystemsWindows 11, Ubuntu 22.04, Kali LinuxVirtualizationVirtualBox


## Currently

- 📚 Finishing my Masters in Information Systems Management
- 🔨 Building more projects and adding them here
- 📖 Working towards CompTIA Security+



## Let's connect

- 💼 [LinkedIn](https://linkedin.com/in/aniket-patel-253820253)
  



*Everything here is built in a home lab for learning purposes. All attacks are performed on systems I own and control.*
