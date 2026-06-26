# Multi-OS Network Lab

## Overview

This repository documents my personal IT home lab environment built using virtual machines running Windows, Ubuntu, and Kali Linux.

The purpose of this lab is to develop skills in:

- Windows Administration
- Linux Administration
- Networking
- Virtualization
- SSH Remote Access
- System Troubleshooting
- Security Fundamentals
- Cross-Platform Integration

---

## Lab Environment

| Operating System | Purpose |
|-----------------|----------|
| Windows 11 | Administration, connectivity testing, and traffic generation |
| Ubuntu Linux | SSH server and Linux system administration |
| Kali Linux | Network discovery, packet analysis, and security testing |

---

## Technologies Used

- VirtualBox
- Windows 11
- Ubuntu Linux
- Kali Linux
- OpenSSH Server
- Nmap
- Wireshark
- TCP/IP Networking
- ICMP
- Git
- GitHub

---

## Tools Used in This Lab Series

- VirtualBox (virtual machine networking and isolation)
- Linux Terminal (Ubuntu + Kali)
- Windows Command Prompt / IP configuration tools
- OpenSSH (secure remote access)
- Nmap (network discovery and scanning)
- Wireshark (packet capture and analysis)
- Ping / ICMP troubleshooting

---

## Project Goals

- Configure communication between multiple operating systems
- Practice troubleshooting network and system issues
- Implement secure remote administration using SSH
- Perform network discovery and service enumeration
- Capture and analyze network traffic
- Document findings using professional technical documentation

---

## Network Configuration

All virtual machines are connected using a Host-Only Adapter in VirtualBox to provide isolated communication between systems.

## Network Architecture

All virtual machines communicate through a VirtualBox Host-Only network, creating an isolated internal environment for safe testing of networking, system administration, and security tools without external network exposure.

---

### Current IP Addresses

| System | IP Address |
|----------|----------|
| Windows 11 | 192.168.56.106 |
| Ubuntu Linux | 192.168.56.101 |
| Kali Linux | 192.168.56.104 |

---

## Skills Demonstrated

- Virtual machine configuration
- TCP/IP networking
- Host-Only network configuration
- Network troubleshooting
- Linux command-line administration
- Windows system administration
- SSH remote administration
- Network discovery with Nmap
- Packet capture and analysis using Wireshark
- Technical documentation
- Cybersecurity fundamentals

---

## Key Achievements

- Built a multi-VM isolated network environment using VirtualBox
- Successfully implemented SSH remote administration between Linux systems
- Performed network discovery and port scanning using Nmap
- Captured and analyzed real network traffic using Wireshark
- Resolved network connectivity issues through systematic troubleshooting

---

## Lab Progress

| Lab | Status |
|-----|--------|
| Network Troubleshooting | Completed |
| SSH Administration | Completed |
| Nmap Network Discovery | Completed |
| Wireshark Traffic Analysis | Completed |
| Linux User & Permissions | Planned |

---

## Repository Structure

```text
multi-os-network-lab/
├── README.md
├── documentation/
│   ├── network-troubleshooting-log.md
│   ├── ssh-administration-lab.md
│   ├── nmap-network-discovery-lab.md
│   └── wireshark-traffic-analysis-lab.md
└── screenshots/
    ├── networking/
    ├── ssh/
    ├── nmap/
    └── wireshark/
```

---

## Documentation

### Completed Labs

- [Network Troubleshooting Log](documentation/network-troubleshooting-log.md)
- [SSH Administration Lab](documentation/ssh-administration-lab.md)
- [Nmap Network Discovery Lab](documentation/nmap-network-discovery-lab.md)
- [Wireshark Traffic Analysis Lab](documentation/wireshark-traffic-analysis-lab.md)

---

## Evidence

### Network Configuration

#### Windows IP Configuration
![Windows IP Configuration](screenshots/networking/windows-ipconfig.png)

#### Ubuntu IP Configuration
![Ubuntu IP Configuration](screenshots/networking/ubuntu-ip.png)

#### Kali IP Configuration
![Kali IP Configuration](screenshots/networking/kali-ip.png)

#### Network Connectivity Test
![Windows Ping Success](screenshots/networking/windows-ping-success.png)

---

## Project Status

### Completed

- Multi-VM environment deployment
- Host-Only network configuration
- Cross-platform connectivity validation
- Network troubleshooting
- SSH remote administration
- Network discovery using Nmap
- Packet capture and analysis using Wireshark

---

### Currently Building

- Linux User and Group Management
- Linux File Permissions
- Firewall Configuration (UFW)

---

### Planned Future Labs

- Apache Web Server Deployment
- DNS Traffic Analysis
- System Log Analysis
- Vulnerability Scanning
- Metasploitable 2 Integration
- Active Directory Lab

---

## Summary

This project demonstrates hands-on experience building and maintaining a multi-operating system virtual lab environment using Windows 11, Ubuntu Linux, and Kali Linux.

The lab covers practical skills in network configuration, system administration, remote access, network discovery, and packet analysis using industry-standard tools such as OpenSSH, Nmap, and Wireshark.

This environment simulates real-world IT and cybersecurity scenarios commonly found in enterprise networks, including troubleshooting connectivity issues, analyzing traffic, and identifying active services across multiple systems.

The project is continuously expanded through additional labs focused on Linux administration, networking, and cybersecurity fundamentals.

These skills are directly applicable to IT support, system administration, network engineering, and cybersecurity analyst roles.
