# Scan_LocalNetwork_for_OpenPorts-
This project scans your local network using Nmap to detect live hosts and open ports. It helps identify running services and potential security risks. The results are saved in a text file for analysis. Useful for beginners in ethical hacking, penetration testing, and network reconnaissance practice.

This project demonstrates a basic network scanning and enumeration process using Nmap on Kali Linux. It is designed for beginners to learn how to identify active hosts, open ports, and potential vulnerabilities within a local network.

📋 Steps Performed:
Install Nmap:

Download and install Nmap from the official website or using apt install nmap on Kali Linux.

Find Local IP Range:

Use ip a or hostname -I to identify your machine’s IP and subnet (e.g., 192.168.1.0/24).

Run TCP SYN Scan:

Execute nmap -sS 192.168.1.0/24 to perform a stealth SYN scan across all devices on the local network.

Identify Live Hosts and Open Ports:

Note down the IP addresses of responsive devices and the list of open TCP ports on each.

Optional – Analyze Traffic with Wireshark:

Use Wireshark to capture and analyze packets during the scan for deeper inspection.

Service Enumeration:

Research the common services running on discovered ports (e.g., SSH on port 22, HTTP on port 80).

Risk Assessment:

Assess the security implications of open ports (e.g., unprotected FTP, exposed database services).

Save Results:

Use -oN scan.txt or -oX scan.xml to export the scan results in text or XML format:

bash
Copy
Edit
nmap -sS 192.168.1.0/24 -oN scan.txt
🛠 Tools Used:
Kali Linux

Nmap

Wireshark (Optional)

🧠 Goal:
To provide a hands-on approach to basic network reconnaissance and lay the foundation for vulnerability scanning and penetration testing.
