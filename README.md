## Hello World!👋

## 📖 𝙰𝚋𝚘𝚞𝚝 𝙼𝚎
- 🌱 I’m currently in my 3rd year of studying Digital Forensics & Cyber Security at TU Dublin
- 🔭 I’m currently working as a tutor in a variety of computing modules for other students at TU Dublin
- 🤔 I’m looking for a work placement as part of my university program
- 😄 Pronouns: she/her
- ⚡ Fun fact: I am bilingual in English and French

## 📫 How to reach me:
[<img src="https://img.icons8.com/color/48/000000/linkedin.png" width="3.5%"/>](https://www.linkedin.com/in/roisinaylward/)  &nbsp; <a href="mailto:roisin.aylward7@gmail.com"> <img src="https://img.icons8.com/fluent/48/000000/gmail.png" width="3.5%"/>

## 👨🏻‍💻 Languages and Tools
<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png"></code>
<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/java/java.png"></code>
<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/mysql/mysql.png"></code>
<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/powershell/powershell.png"></code>
<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/bash/bash.png"></code>
<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/docker/docker.png"></code>
<code><img height="40" src="https://github.com/github/explore/blob/main/topics/claude/claude.png"></code>
<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/aws/aws.png"></code>
<code><img height="40" src="https://github.com/github/explore/blob/main/topics/azure/azure.png"></code>
<code><img height="40" src="https://upload.wikimedia.org/wikipedia/commons/d/db/Oracle-cloud-infrastructure.png"></code>

## 🎓 Academic & Course Projects
### 📈 2nd Year Modules:

* [Cyberattack Detection with Machine Learning (COMP H2706)](https://github.com/RoisinAylward/CyberattackDetectionML) - A CRISP-DM data science project analysing 6,000 network sessions to detect brute-force attacks against a financial organisation. Built for *Fundamentals of AI & Data Science*.
  * **ML Stack:** Python notebook built on pandas, NumPy and scikit-learn, with Matplotlib and seaborn for exploratory visualisation.
  * **Data Quality & Preparation:** Detected and resolved inconsistent protocol labels, logically impossible records (e.g. failed logins exceeding total attempts), 7% missing values and outliers, using distribution-aware imputation and IQR capping.
  * **Feature Engineering:** Designed three security-driven features: login failure rate (brute-force intensity), sent/received byte ratio (possible exfiltration) and retry rate (possible scanning). The byte ratio ranked as the second most important attack predictor.
  * **Modelling & Evaluation:** Compared Decision Tree and KNN classifiers for `attack_category`, and Linear Regression and Decision Tree Regressor for `avg_packet_size`, using stratified hold-out testing, 5-fold cross-validation, confusion matrices and RMSE/MAE/R².
  * **Documentation:** Includes the full [Project Report (PDF)](https://github.com/RoisinAylward/CyberattackDetectionML/blob/main/documentation/Project_Report_B00168689.pdf) viewable natively in-repo.

* [Secure AWS Cloud Architecture: WinLocal Giveaways (COMP H2701)](https://github.com/RoisinAylward/WinLocalCloudArchitecture) - Designed a secure, scalable AWS architecture for a fictional Dublin start-up recovering from a ransomware attack, and built a proof of concept of it in an AWS Academy Learner Lab. Built for *Security Architecture*.
  * **Architecture:** draw.io design across two Availability Zones with public and private subnets, a bastion host, NAT gateway, Application Load Balancer, Auto Scaling, RDS MySQL and an S3 static backup website.
  * **Network Security:** Four least-privilege security groups chained bastion to web to database, plus stateless network ACLs on every subnet. The web servers and database have no public access.
  * **Scalability:** Auto Scaling group with a target tracking policy holding average CPU at 60%, launching from a custom AMI. A load test triggered scale-out to a second instance.
  * **Beyond the PoC:** Justified IAM (least privilege per role and MFA) and Route 53 DNS failover to the S3 backup site, and evaluated the design against the AWS Well-Architected Sustainability Pillar.
  * **Group Work:** NIST CSF 2.0 security posture presentation for the business owners with Sofiia Prymak and Livia Mathew, where I covered the recommended controls for all six functions.
  * **Documentation:** Includes the full [Report (PDF)](https://github.com/RoisinAylward/WinLocalCloudArchitecture/blob/main/documentation/Report_B00168689.pdf) and [Presentation (PDF)](https://github.com/RoisinAylward/WinLocalCloudArchitecture/blob/main/documentation/AWS%20Cloud%20Infrastructure%20Deployment.pdf) viewable natively in-repo.

* [OWASP Juice Shop Security Assessment (COMP H2704)](https://github.com/RoisinAylward/JuiceShopSecurityAssessment) - Attacked OWASP Juice Shop, a deliberately insecure web shop, then analysed the vulnerabilities behind the challenges and tested the app with Semgrep (SAST) and OWASP ZAP (DAST). Built as a group project for *Web Application Security*.
  * **Exploitation:** Solved Database Schema, User Credentials, Two-Factor Authentication, Reset Jim's Password and Forgotten Developer Backup using UNION-based SQL injection, OSINT and a null byte bypass.
  * **Vulnerability Analysis:** Traced SQL injection (CWE-89) to raw template-literal queries in `routes/search.ts` and `routes/login.ts`, and broken authentication (CWE-287) to security-question resets and plaintext TOTP secrets, with mitigations mapped to OWASP ASVS 5.0 and the Proactive Controls.
  * **SAST:** Ran Semgrep through Docker (302 rules on 2096 files), sorted out duplicate findings and false positives, and linked its path traversal (CWE-22) and directory listing (CWE-548) findings to the Forgotten Developer Backup challenge.
  * **DAST:** Validated ZAP findings by hand in the browser: a stack trace leak from `/api/`, a wildcard CORS policy and a session ID exposed in `socket.io` URLs.
  * **Documentation:** Includes the full [Technical Report (PDF)](https://github.com/RoisinAylward/JuiceShopSecurityAssessment/blob/main/documentation/Report_32.pdf) and my [ZAP Scan Report (PDF)](https://github.com/RoisinAylward/JuiceShopSecurityAssessment/blob/main/dast/2026-05-05-ZAP-Report-localhost.pdf) viewable natively in-repo, plus the full Semgrep output.

* [Threat Hunter Toolkit (COMP H2705)](https://github.com/RoisinAylward/ThreatHunterToolkit) - An Automated SOC Investigation Framework engineered to process high-volume security logs and automatically flag cross-platform indicators of compromise. Built for *Advanced Scripting for Cyber Security*.
  * **Automation Stack:** Native PowerShell orchestration core (`run.ps1`) driving high-throughput pattern matching and string manipulation across log files.
  * **Multi-Source Log Analysis:** Ingests and correlates disparate log data streams including web server entries (`access.log`), Linux/SSH authentication attempts (`auth.log`), and native host activities (`powershell_log.txt`).
  * **Threat Intelligence Cross-Checking:** Automates malicious indicator validation by cross-referencing extracted host/network data directly against internal Threat Intel databases (`ioc.txt`).
  * **Detection Logic Engine:** Implements threshold-based alerts targeting brute-force authentication models, anomalous obfuscation patterns (e.g., `-EncodedCommand`), and data exfiltration pipelines.
  * **Reporting Architecture:** Outputs structured, timestamped triage records dynamically catalogued in an analytical `archive/` database.
  * **Documentation:** Includes the full [Threat Hunter Toolkit  Report (PDF)](https://github.com/RoisinAylward/ThreatHunterToolkit/blob/main/documentation/Threat%20Hunter%20Toolkit%20Report.pdf) viewable natively in-repo.

* [Secure Azure Cloud Deployment: TechStart Solutions (COMP H2703)](https://github.com/RoisinAylward/techstartsolutions) - Designed, deployed and secured the Azure infrastructure for a fictional six-person software company's web app, covering network segmentation, least-privilege access control, encryption, Linux hardening, logging and backups. Built for *Security Administration*.
  * **Cloud Stack:** Ubuntu 24.04 VM running Apache, mod_wsgi and Flask, with Azure SQL Database, Blob Storage and Key Vault, inside one VNet split into three subnets.
  * **Network Segmentation:** Least-privilege NSG rules (SSH from my IP only, web traffic on 80/443 only), with the database and Key Vault closed to the internet and reachable only through private endpoints.
  * **Authentication & Access Control:** SSH key-only login with root login disabled, PAM account lockout (`pam_faillock`), password complexity, history and ageing rules, and Azure RBAC roles mapped to the Developer, QA and Project Manager teams.
  * **Encryption:** TDE on Azure SQL, encryption at rest on Blob Storage, TLS 1.2 minimum for database connections, and HTTPS with an HTTP-to-HTTPS redirect.
  * **Hardening & Monitoring:** UFW default-deny firewall with SSH rate limiting, Fail2ban, automatic security updates, and a Bash security monitoring script (`security_monitor.sh`).
  * **Logging & Backups:** Persistent journald and logrotate retention policies, Azure SQL automated backups, and a nightly cron job that backs up the web server.
  * **Documentation:** Includes the full [Project Report (PDF)](https://github.com/RoisinAylward/techstartsolutions/blob/main/documentation/SecurityAdministrationProjectReport.pdf) viewable natively in-repo.

* [Modular Incident Response Triage (MIRT) Toolkit (COMP H2702)](https://github.com/RoisinAylward/MIRT) - A plugin-based, multi-language mini DFIR framework that automates basic incident response triage on Windows. Built as a group project for *Scripting for Cyber Security*.
  * **Automation Stack:** A PowerShell collector (`collector.ps1`) and orchestrator built by my teammate, feeding a Python 3 analysis core (`mirt.py`) that I built.
  * **Threat Intel & Enrichment:** My plugins check file hashes against VirusTotal and public IPs against AbuseIPDB, with caching and rate limiting. A persistence plugin we designed together flags Run-key entries in user-writable paths.
  * **Detection Focus:** Targets Windows Run-key persistence and hunts PowerShell logs for encoded commands (`-EncodedCommand`) and other suspicious keywords.
  * **Outcome:** Tested end-to-end on a real Windows laptop: checked 5 executable hashes on VirusTotal and flagged 2 Run-key entries in AppData, with every finding in a Markdown report grouped by severity.
  * **Documentation:** Includes the full [Technical Report (PDF)](https://github.com/RoisinAylward/MIRT/blob/main/documentation/Technical%20Report.pdf) natively viewable in-repo.
 
* [Open-Source Firewalls: OPNsense, IPCop & IPFire (CYSC H1001)](https://github.com/RoisinAylward/OpenSourceFirewalls) - Each of us set up a different open-source firewall in the same virtual testbed, attacked it from the WAN side, hardened it, and ran the same attacks again to compare all three. Built as a group project for *Network Security*.
  * **My Part:** Configured and tested IPCop, managed from an Xubuntu VM on the internal network and attacked from a Kali Linux VM.
  * **Testbed:** Each firewall separated a WAN with the attacker, a DMZ with a port-forwarded Apache web server, and an internal network.
  * **Attacks:** Nmap reconnaissance scans, ICMP floods with hping3 (including random source IPs), HTTP floods with wrk, and SSH brute forcing with Hydra and the RockYou wordlist.
  * **Hardening:** Dropped ICMP from the untrusted (red) network, moved HTTP traffic to a lower traffic-shaping priority, and closed SSH to the red network. Afterwards the wrk flood fell from 190.84MB to 2.30MB of traffic in 20 seconds, and Hydra could no longer reach SSH.
  * **Documentation:** Includes the full [Project Report (PDF)](https://github.com/RoisinAylward/OpenSourceFirewalls/blob/main/documentation/B00168689RoisinAylwardnetsecurity.pdf) and [Presentation (PDF)](https://github.com/RoisinAylward/OpenSourceFirewalls/blob/main/documentation/Network%20Security%20Project%20Presentation.pdf) viewable natively in-repo.
 
* [Hospital Database (COMP H1029)](https://github.com/RoisinAylward/HospitalDatabase) - Designed and built a MySQL database for a hospital, from conceptual, logical and physical ER diagrams through to a 10-table schema in third normal form and 20 SQL tasks. Built for *Database Fundamentals*.
  * **Design:** Entities, business rules, cardinalities and participation constraints, worked from a conceptual ERD through a logical ERD to a physical model in MySQL Workbench.
  * **Schema:** 10 tables covering departments, treatments, staff, patients, medical history, contact details, bed allocation and appointments, with composite keys and junction tables for the many-to-many relationships.
  * **Data:** DDL and DML scripts that create the database and fill every table with between 11 and 53 rows of sample data.
  * **SQL:** 20 tasks using joins across up to five tables, aggregates, date arithmetic, updates, deletes that respect foreign keys, and a view that draws on three tables.
  * **Documentation:** Includes the full [Project Report (PDF)](https://github.com/RoisinAylward/HospitalDatabase/blob/main/documentation/DBF_project_report.pdf) viewable natively in-repo.


### 📈 1st Year Modules:
* [Contact Book Application (COMP H1031)](https://github.com/RoisinAylward/contact_book) - A Python-based contact management system utilising CSV file storage. Built as the final project for *Fundamentals of Python Programming 2*.
  * **Core Architecture:** Split into `main.py` for user interface execution and `core_logic.py` for backend processing.
  * **Security & Reliability Focus:** Implemented robust input data validation and sanitisation techniques to protect against malformed data entry.
  * **Testing Suite:** Comprehensive unit tests (`test_core_logic.py`) to automate input validity checking and ensure functional consistency.



## 🛠️ Personal Side Projects 
* [Smart Camera (WIP)](https://github.com/RoisinAylward/smartcamera) - A work in progress for a self-hosted home security setup that includes alarms, indoor & outdoor cameras, and a video and two-way intercom doorbell. All devices are hosted both locally and in the cloud, and are connected to a control centre mobile application.
* [Minecraft Server (WIP)](https://github.com/RoisinAylward/minecraft-server) - A work in progress for an Archery-themed Minecraft Server with mods and plugins.

<!--
**RoisinAylward/RoisinAylward** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
