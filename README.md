# networkwalks_zenmap-and-the-harvester-foot-printing-report
Cybersecurity Reconnaissance and Network Discovery Project
Overview
This project combines passive OSINT reconnaissance with theHarvester and authorized local-network host discovery with Zenmap/Nmap.
Tools
Kali Linux 2026.2
theHarvester 4.10.x
Zenmap / Nmap 7.991
Windows Command Prompt
Oracle VirtualBox
Part 1: theHarvester OSINT
Target used in the captured lab exercise: `microsoft.com`.
The captured output reported no IP addresses, emails, people, or hosts. LinkedIn collection returned no users and zero links. SecurityScorecard and BuiltWith enrichment could not complete because API keys were not configured, and Windvane used limited unauthenticated access.
Part 2: Zenmap/Nmap Network Discovery
Command used:
```bash
nmap -sn 192.168.1.0/24
```
The scan covered 256 addresses and reported 6 hosts up. The Windows host configuration showed IPv4 `192.168.1.137`, subnet mask `255.255.255.0`, and default gateway `192.168.1.1`.
Because `-sn` performs host discovery, these results do not establish open ports, services, vulnerabilities, or compromise.
Skills Demonstrated
OSINT, reconnaissance, Nmap/Zenmap, network discovery, IP addressing, host identification, evidence analysis, and cybersecurity reporting.
Repository Structure
```text
cybersecurity-recon-project/
├── README.md
├── reports/
│   └── combined-cybersecurity-report.docx
├── evidence/
│   ├── theharvester/
│   └── nmap-zenmap/
└── notes/
    └── methodology.md
```
Responsible Use
Only perform security testing on systems and networks you own or have explicit permission to assess. Do not publish passwords, API keys, tokens, or sensitive network information.
