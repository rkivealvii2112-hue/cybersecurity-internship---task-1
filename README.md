# cybersecurity-internship---task-1
# Cyber Security Internship - Task 1: Scan Your Local Network for Open Ports 

## Objective
]To discover open ports on devices within the local network to analyze network service exposure and understand potential vulnerabilities.

## Tools Used
**Nmap**: Used to perform a stealthy TCP SYN scan across the local subnet. [cite: 7, 11]
- **Windows PowerShell (Admin)**: Executed the command-line network scan.

## Methodology & Execution
1. dentified the active local network subnet range (`192.168.1.0/24`) using network configuration commands (`ipconfig`).
2.]Executed a TCP SYN stealth scan to check for active hosts and open ports. 
   ```bash
   .\nmap.exe -sS -oN scan_results.txt 192.168.1.0/24
