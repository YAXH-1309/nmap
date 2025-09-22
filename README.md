# nmap
A repository documenting the process of scanning a local network for open ports, including the tools used, the methodology, and an analysis of the findings and associated security risks.
Network Reconnaissance: Local Port Scan
Overview
This project documents the first task of the cybersecurity internship: to perform a port scan on a local network. The objective was to gain foundational knowledge of network reconnaissance, understand how services are exposed on a network, and identify potential security risks.

Tools Used
Nmap: A free and open-source utility used for network discovery and security auditing.   

PowerShell: The command-line interface used to execute the scan command.

Process
Identified Local IP Range: I used a command-line utility to determine the IP address and subnet of my local network.

Executed a TCP SYN Scan: I ran the Nmap command nmap -sS <my_ip_range> to perform a stealth scan and identify all open ports and live hosts on the network.   

Saved and Converted Results: The scan results were saved in XML format using the -oX flag. I then used the xsltproc utility to convert the XML output to a formatted HTML report for easy viewing and analysis.

Findings
The scan successfully identified several open ports on a device on the local network. These ports are associated with common network services, including:

Port 80 (HTTP)

Ports 135, 139, and 445 (Microsoft services, including SMB and NetBIOS)

Port 1801 (Microsoft Message Queuing)

Port 2103 (Zephyr Notification Service)

Port 2105 (Eklogin, an encrypted remote login service)

Port 2107 (MSMQ management)

Port 5432 (PostgreSQL database)

Conclusion
This task was crucial for understanding how to identify a network's attack surface. By identifying these open ports, I was able to see how services are exposed and learn about the security risks associated with them, such as vulnerabilities in outdated services. The process of documenting the scan reinforces the importance of professional reporting in cybersecurity.
