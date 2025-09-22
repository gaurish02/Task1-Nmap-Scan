# Task 1 — Nmap Network Scan

## Objective
Scan the local network to identify active hosts and open ports.

## Tools Used
- Nmap
- Windows Command Prompt

## Command Run
nmap -sS 192.168.X.X/24

## Files in this Repo
- scan_results.txt → Nmap output
- screenshot1.png → Terminal showing Nmap command
- screenshot2.png → Example of open ports


## Key Findings
- **192.168.1.1** → Ports 53 (DNS), 80 (HTTP), 443 (HTTPS) open; 22 & 23 filtered  
- **192.168.1.2** → All scanned ports closed  
- **192.168.1.4** → All scanned ports closed  
- **192.168.1.7** → Ports 135 (MSRPC), 139 (NetBIOS-SSN), 445 (Microsoft-DS), 6646 open  
- **192.168.1.8** → Ports 8008, 8009, 8443, 9000 open

## Security Risks & Suggestions
- Close unnecessary ports to reduce attack surface.  
- Use strong authentication on services like MSRPC, NetBIOS, and HTTP.  
- Consider firewall rules to filter unused ports.  
