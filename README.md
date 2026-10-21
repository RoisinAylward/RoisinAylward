## Hello World!👋

## 📖 𝙰𝚋𝚘𝚞𝚝 𝙼𝚎
- 🌱 I’m currently in my 3rd year of studying Computer Science at TU Dublin, with a special interest in Digital Forensics & Cybersecurity
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
  * **Documentation:** Includes the full [Project Report (PDF)](Project_Report_B00168689.pdf) viewable natively in-repo.

* [Threat Hunter Toolkit (COMP H2705)](https://github.com/RoisinAylward/ThreatHunterToolkit) - An Automated SOC Investigation Framework engineered to process high-volume security logs and automatically flag cross-platform indicators of compromise. Built for *Advanced Scripting for Cyber Security*.
  * **Automation Stack:** Native PowerShell orchestration core (`run.ps1`) driving high-throughput pattern matching and string manipulation across log files.
  * **Multi-Source Log Analysis:** Ingests and correlates disparate log data streams including web server entries (`access.log`), Linux/SSH authentication attempts (`auth.log`), and native host activities (`powershell_log.txt`).
  * **Threat Intelligence Cross-Checking:** Automates malicious indicator validation by cross-referencing extracted host/network data directly against internal Threat Intel databases (`ioc.txt`).
  * **Detection Logic Engine:** Implements threshold-based alerts targeting brute-force authentication models, anomalous obfuscation patterns (e.g., `-EncodedCommand`), and data exfiltration pipelines.
  * **Reporting Architecture:** Outputs structured, timestamped triage records dynamically catalogued in an analytical `archive/` database.
  * **Documentation:** Includes the full [Threat Hunter Toolkit  Report (PDF)](https://github.com/RoisinAylward/ThreatHunterToolkit/blob/main/documentation/Threat%20Hunter%20Toolkit%20Report.pdf) viewable natively in-repo.

* [Modular Incident Response Triage (MIRT) Toolkit (COMP H2702)](https://github.com/RoisinAylward/MIRT) - A plugin-based, multi-language mini DFIR framework designed to automate host-based incident response triage on Windows environments. Built as a group project for *Scripting for Cyber Security*.
  * **Automation Stack:** Combines a Windows PowerShell collector core (`collector.ps1`) with a multi-threaded Python 3 analysis engine (`mirt.py`).
  * **Threat Intel & Enrichment:** Features a dynamic plugin architecture utilising the VirusTotal and AbuseIPDB APIs for automated hash reputation, IP enrichment, and suspicious persistence detection.
  * **Detection Focus:** Targets Windows Run keys and common defence evasion techniques, such as parsing heavily obfuscated and base64-encoded PowerShell payloads.
  * **Documentation:** Includes the full [Technical Report (PDF)](https://github.com/RoisinAylward/MIRT/blob/main/documentation/Technical%20Report.pdf) natively viewable in-repo.


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
