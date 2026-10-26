NETWORKMINER-PROJECT

THIS IS MY NETWORKMINER HANDS ON PRACTICAL PROJECT WITH TRYHACKME

Network Forensics & Protocol Analysis Lab: NetworkMiner Capstone. A hands-on network forensics and passive traffic analysis project completed through TryHackMe, focusing on PCAP parsing, credential harvesting, host fingerprinting, and extracted object analysis using NetworkMiner.

Table of Contents
Project Overview
Operating Modes & Data Types
Tools & Technologies Used
Key Investigation Areas
Conclusion

📌 Project Overview

NetworkMiner is an important open-source Network Forensic Analysis Tool (NFAT). It acts as a passive sniffer that fingerprints host OS, active sessions, open ports, and extracted network artifacts without injecting traffic into the network. It also serves as a PCAP parser that reassembles files, certificates, and messages from captured traffic for forensic analysis.

⚙️ Operating Modes & Data Types

Data Types Captured & Parsed:
Live Traffic
Log Files
Traffic Captures (PCAPs)
Operational Modes:
Sniffer Mode: Used for passive packet sniffing and live network traffic capturing.
Packet Snarfing / Processing Mode: Used to grab high-value artifacts ("low-hanging fruit") from PCAP files before conducting deeper packet-level investigations.

🛠️ Tools & Technologies Used

NetworkMiner: (Passive sniffing, PCAP parsing, protocol analysis, OS fingerprinting, extracted file/image reassembly, credential grabbing)

Linux Terminal: (Path navigation and exercise file management)

TryHackMe: (Forensics lab environment and target PCAP capture files)

🔍 Key Investigation Areas

Reconnaissance & Host Fingerprinting: Passive OS fingerprinting, MAC address association, and web server banner identification across network endpoints.

Authentication & Credential Extraction: Harvesting cleartext credentials, domain usernames, and NTLM password hashes directly from captured protocol artifacts.

Artifact Navigation & Anomaly Detection: Extracted file metadata examination, embedded image source tracing, and TLS anomaly identification.

Mail & Communication Forensics: Reconstructing email headers, message contents, and user email identities from unencrypted session traffic.

Deep Session Metrics & Device Profiling: Port-level byte transfer calculations, TCP sequence number analysis, USB/hardware brand identification, and DNS query mapping.

🛡️ Conclusion

NetworkMiner is an essential tool for starting a network security investigation and traffic inspection. However, deeper analysis tools and layered defenses are necessary to completely mitigate active threats.
