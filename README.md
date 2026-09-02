# Cyber Security SOC Lab 🛡️

Welcome to my first Cyber Security SOC (Security Operations Center) Lab In this project, I built a complete environment to simulate cyber attacks, monitor activities, and analyze logs like a real security analyst.
------------------------------------------------------------------------------------------------------------------------------
# 🗺️ The Story & Architecture
Think of this lab as a story with three main characters:
1. The Attacker (Kali Linux):** The machine used to launch security attacks.
2. The Victim (Windows 10):** The target machine, equipped with **Sysmon** (using Olaf Hartong's modular config) to watch every single movement in the background.
3. The Receiver / SIEM (Splunk on Ubuntu):** The brain of the operation that collects all the logs and helps us analyze them.
------------------------------------------------------------------------------------------------------------------------------
# 🚀 What I Have Done So Far
I have successfully built the core infrastructure of this lab:
* **Configured the Victim (Windows 10):** Installed **Sysmon** and applied the smart **Olaf Hartong configuration** to filter and tag high-quality security events.
* **Set up the Shipper:** Configured **Splunk Universal Forwarder** on Windows 10 to securely ship security and Sysmon logs through the network.
* **Prepared the Receiver (Ubuntu Server):** Activated Splunk Enterprise on Ubuntu, opened **Port 9997** to listen for incoming data, and created dedicated indexes (`sysmon` and `wineventlog`) to store the logs safely.
---------------------------------------------------------------------------------------------------------------------------
# 📊 Lab Status: Connected & Running!
The backend setup is 100% complete and working:
* **Sysmon Service:** Active & Monitoring.
* **SplunkForwarder Service:** `Running` and successfully connected to the Ubuntu server.
* **Splunk Server:** Active and waiting to visualize the data.
*Next Step: Generating cyber attacks from Kali Linux and tracing them inside the Splunk dashboard!*
---------------------------------------------------------------------------------------------------------------------------
