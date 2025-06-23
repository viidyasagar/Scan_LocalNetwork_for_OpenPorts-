# Scan_LocalNetwork_for_OpenPorts-
This project scans your local network using Nmap to detect live hosts and open ports. It helps identify running services and potential security risks. The results are saved in a text file for analysis. Useful for beginners in ethical hacking, penetration testing, and network reconnaissance practice.

This project showcases a beginner-friendly approach to network scanning and enumeration using Nmap on Kali Linux. It's designed to help new cybersecurity learners identify live hosts, open ports, and potential vulnerabilities within a local network.

🧭 Steps Followed
1️⃣ Install Nmap
🔗 Download and install Nmap from the official website
Or run:

bash
Copy
Edit
sudo apt update && sudo apt install nmap
2️⃣ Find Your Local IP Range
📡 Use the following commands to find your local IP and subnet:

bash
Copy
Edit
ip a
hostname -I
➡️ Example output: 192.168.1.10/24 → This means your scan range is 192.168.1.0/24.

3️⃣ Perform a TCP SYN Scan
🚀 Run a stealth scan using:

bash
Copy
Edit
nmap -sS 192.168.1.0/24
This will discover live devices and their open TCP ports.

4️⃣ Note IPs & Open Ports
📝 Record all live IP addresses and the corresponding open ports found during the scan.

5️⃣ (Optional) Analyze with Wireshark
🔬 Capture traffic using Wireshark during the scan to see how packets interact at a deeper level.

6️⃣ Research Common Services
🧠 Look up what services run on open ports (e.g., 22 = SSH, 80 = HTTP) to understand potential exposures.

7️⃣ Identify Security Risks
⚠️ Analyze which ports/services may present vulnerabilities, especially if unprotected or outdated.

8️⃣ Save Scan Results
💾 Store your scan results for documentation or analysis:

bash
Copy
Edit
nmap -sS 192.168.1.0/24 -oN scan.txt
You can also export in XML or HTML using -oX or -oA flags.

🛠 Tools Used
🐱 Kali Linux

🛰️ Nmap

🐬 Wireshark (optional)

🎯 Goal
To build a foundational understanding of how to:

Scan a network

Discover live systems

Investigate services and open ports

Assess basic vulnerabilities
