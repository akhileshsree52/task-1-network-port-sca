# Task 1: Local Network Port Scanning

## Objective
To identify open ports and services on devices in my local network using Nmap.

## Tool Used
- Nmap (TCP SYN Scan)

## Command Executed
```bash
sudo nmap -sS 192.168.1.39/24

Findings

The scan identified multiple active hosts within the local network IP range. One of the primary devices (192.168.1.1) had the following open ports:

21/tcp (FTP)

53/tcp (DNS)

80/tcp (HTTP)

443/tcp (HTTPS)

Some ports such as 22n(SSH), 23 (Telnet), 139, and 445 were filtered, indicating firewall protection.

The detailed scan output is saved in the file scan_results.txt included in this repository.

Security Analysis

FTP (21) may expose credentials if not secured.

HTTP (80) transmits data in plaintext.

HTTPS (443) provides encrypted communication.

Filtered ports indicate firewall rules are active.

Learning Outcome

Learned how to perform TCP SYN scans

Understood network service exposure

Gained basic network reconnaissance skills


