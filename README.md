# So-You-Want-To-Be-a-SOC-Analyst

https://blog.ecapuano.com/p/so-you-want-to-be-a-soc-analyst-intro

Overview
This lab provided a practical introduction to building a cloud-based SOC environment, simulating real-world attack scenarios, and using tools like Azure Sentinel and LimaCharlie for threat detection and response.

Lab Components
1. Environment Setup
•	Cloud-Based Virtual Machine: Deployed a pre-configured, cloud-hosted VM, eliminating the need for local setup.
•	LimaCharlie EDR Integration: Installed the LimaCharlie Endpoint Detection and Response (EDR) agent to monitor system activities and collect security telemetry.

2. Command and Control (C2) Simulation
•	Sliver C2 Framework: Set up a Sliver Command and Control (C2) server within the VM to simulate adversarial operations.
•	Payload Deployment: Created and executed payloads to establish C2 sessions, mimicking common attack vectors.

3. Adversarial Activities
•	Privilege Escalation: Simulated techniques used by attackers to gain elevated system privileges.
•	Credential Dumping: Extracted sensitive data, including dumping the lsass.exe process, to understand data exposure risks.

4. Detection and Response
•	LimaCharlie Telemetry Analysis: Monitored and analyzed security events to identify potential compromises.
•	Custom Detection Rules: Developed and implemented rules to detect malicious activities, improving threat detection.
•	Blocking Malicious Actions: Configured automated responses to prevent threats, such as blocking the deletion of volume shadow copies—a common ransomware tactic.

5. Advanced Threat Detection
•	Automated YARA Scanning: Integrated YARA rules to scan for known malware signatures, enhancing file and process threat detection.

Key Learnings
Adversarial Simulations – Used the Sliver C2 framework to replicate real-world attack techniques, such as reconnaissance and C2 sessions, gaining insights into attacker methodologies.
Detection and Response – Built and tested detection rules in Azure Sentinel, while monitoring endpoint activity in LimaCharlie, to proactively identify and respond to threats.
Blocking Threats – Configured LimaCharlie rules to block payload execution and prevent unauthorized access to critical processes like lsass.exe.

