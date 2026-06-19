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

## Lab Environment

| Operating System | Purpose |
|-----------------|----------|
| Windows 11 | Administration and file sharing |
| Ubuntu Linux | Server administration and remote access |
| Kali Linux | Network diagnostics and security testing |

## Technologies Used

- VirtualBox or VMware
- Windows 11
- Ubuntu Linux
- Kali Linux
- SSH
- TCP/IP Networking
- Nmap
- Wireshark
- Git
- GitHub

## Project Goals

- Configure communication between multiple operating systems
- Practice troubleshooting network and system issues
- Implement secure remote administration
- Analyze network traffic
- Document findings and solutions

## Network Configuration

All virtual machines are connected using a Host-Only Adapter in VirtualBox to provide isolated communication between systems.

### Current IP Addresses

| System | IP Address |
|----------|----------|
| Windows 11 | 192.168.56.106 |
| Ubuntu Linux | 192.168.56.101 |
| Kali Linux | 192.168.56.103 |

## Skills Demonstrated

- Network Configuration
- System Administration
- Linux Command Line
- Windows Management
- Troubleshooting
- Documentation
- Security Awareness
- Virtual Machine Networking

## Repository Structure

```text
multi-os-network-lab/
├── README.md
├── documentation/
└── screenshots/
    └── networking/
```

## Documentation

- [Network Troubleshooting Log (Completed)](documentation/network-troubleshooting-log.md)
- SSH Administration Lab (Coming Soon)
- System Administration Notes (Coming Soon)

## Evidence

### Windows IP Configuration
![Windows IP Configuration](screenshots/networking/windows-ipconfig.png)

### Ubuntu IP Configuration
![Ubuntu IP Configuration](screenshots/networking/ubuntu-ip.png)

### Kali IP Configuration
![Kali IP Configuration](screenshots/networking/kali-ip.png)

### Network Connectivity Test
![Windows Ping Success](screenshots/networking/windows-ping-success.png)

## Status

### Completed
- Multi-VM environment deployment
- Host-Only network configuration
- Windows, Ubuntu, and Kali connectivity validation
- Initial troubleshooting documentation

### In Progress
- SSH administration lab
- Linux user management
- Remote system administration

### Planned
- Nmap network discovery
- Wireshark traffic analysis
- Metasploitable 2 integration
- Security hardening exercises

## Summary

This project demonstrates hands-on experience configuring and troubleshooting a multi-operating system virtual lab environment using Windows, Ubuntu Linux, and Kali Linux. Skills practiced include networking, virtualization, remote administration, system troubleshooting, and technical documentation. The lab serves as a foundation for developing IT support, system administration, and cybersecurity skills. The lab is continuously expanded through hands-on projects focused on networking, Linux administration, remote access, and cybersecurity fundamentals.
