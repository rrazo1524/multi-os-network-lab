# Multi-OS Network Lab

![Platform](https://img.shields.io/badge/Platform-VirtualBox-blue)
![OS](https://img.shields.io/badge/OS-Windows%2011%20%7C%20Ubuntu%20%7C%20Kali-success)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

## Overview

The **Multi-OS Network Lab** is a hands-on home laboratory built with VirtualBox to develop practical experience in system administration, networking, Linux administration, security fundamentals, troubleshooting, and technical documentation.

The environment uses multiple operating systems connected through an isolated VirtualBox Host-Only network.

The lab is continuously expanded with additional systems, security tools, administrative tasks, and cybersecurity exercises.

---

## Lab Environment

| System           | Role                    | IP Address        |
| ---------------- | ----------------------- | ----------------- |
| Windows 11       | Client / Administration | `192.168.56.106`  |
| Ubuntu Linux     | Server / SSH / Services | `192.168.56.101`  |
| Kali Linux       | Security Testing        | `192.168.56.104`  |
| Metasploitable 2 | Vulnerable Target       | Planned / Testing |

### Virtualization

* VirtualBox
* Host-Only Networking
* Isolated Lab Environment
* Multiple operating systems
* Cross-platform administration

---

## Network Architecture

```text
                         Host Machine
                              |
                        VirtualBox
                              |
                   Host-Only Network
                     192.168.56.0/24
                              |
        ------------------------------------------------
        |                       |                      |
        |                       |                      |
 [ Windows 11 ]           [ Ubuntu ]             [ Kali ]
  .56.106                   .56.101                .56.104
  Client/Admin              Server                 Security
        |                       |                      |
        |                       |                      |
        ----------- Network Testing ------------------
```

The lab is designed to provide an isolated environment for practicing administration, networking, troubleshooting, and security testing without relying on production systems.

---

# Completed Labs

## Network Troubleshooting

**Documentation:** [Network Troubleshooting Lab](documentation/network-troubleshooting-log.md)

Topics include:

* IP configuration
* Connectivity testing
* ICMP
* Cross-platform troubleshooting
* Network verification
* Systematic troubleshooting methodology

---

## SSH Administration

**Documentation:** [SSH Administration Lab](documentation/ssh-administration-lab.md)

Topics include:

* OpenSSH
* Remote administration
* SSH authentication
* Linux server administration
* Remote command execution
* Connectivity verification

---

## Nmap Network Discovery

**Documentation:** [Nmap Network Discovery Lab](documentation/nmap-network-discovery-lab.md)

Topics include:

* Host discovery
* Port scanning
* Service identification
* Network enumeration
* Security reconnaissance

---

## Wireshark Traffic Analysis

**Documentation:** [Wireshark Traffic Analysis Lab](documentation/wireshark-traffic-analysis-lab.md)

Topics include:

* Packet capture
* ICMP traffic
* SSH traffic
* Network analysis
* Protocol identification
* Traffic investigation

---

## Linux Permissions

**Documentation:** [Linux Permissions Lab](documentation/linux-permissions-lab.md)

Topics include:

* Linux users
* Groups
* File ownership
* `chmod`
* `chown`
* Permission troubleshooting
* Access control

---

## UFW Firewall Configuration

**Documentation:** [UFW Firewall Configuration Lab](documentation/ufw-firewall-configuration-lab.md)

Topics include:

* UFW
* Firewall rules
* Allow/deny policies
* SSH access
* HTTP access
* FTP blocking
* Network verification

---

## Apache Web Server

**Documentation:** [Apache Web Server Lab](documentation/apache-web-server-lab.md)

Topics include:

* Apache installation
* Linux web server administration
* Service management
* Web server configuration
* HTTP testing

---

# Lab Methodology

Each lab follows a structured workflow:

1. Define the objective
2. Identify the systems involved
3. Configure the environment
4. Select appropriate tools
5. Perform the task
6. Verify the results
7. Troubleshoot unexpected behavior
8. Capture evidence
9. Analyze security implications
10. Document the results

This approach is intended to make the labs reproducible and demonstrate a systematic troubleshooting process.

---

# Technologies & Tools

### Operating Systems

* Windows 11
* Ubuntu Linux
* Kali Linux
* Metasploitable 2

### Networking & Security

* TCP/IP
* ICMP
* SSH
* Nmap
* Wireshark
* UFW
* Network troubleshooting

### Linux Administration

* Bash
* `chmod`
* `chown`
* `useradd`
* `usermod`
* `groupadd`
* OpenSSH
* Apache

### Infrastructure

* VirtualBox
* Host-Only Networking
* Git
* GitHub

---

# Skills Demonstrated

| Skill                   | Demonstrated Through          |
| ----------------------- | ----------------------------- |
| Linux Administration    | Permissions, SSH, UFW, Apache |
| Networking              | Network Troubleshooting, Nmap |
| Packet Analysis         | Wireshark                     |
| Firewall Management     | UFW                           |
| Remote Administration   | SSH                           |
| Access Control          | Linux Permissions             |
| Network Discovery       | Nmap                          |
| Troubleshooting         | Network Troubleshooting       |
| Virtualization          | VirtualBox                    |
| Technical Documentation | All Labs                      |

---

# Security Principles

The lab incorporates several foundational security concepts:

* Least privilege
* Network isolation
* Access control
* Secure remote administration
* Host-based firewalls
* Service exposure
* Network monitoring
* Security testing
* Evidence-based troubleshooting

All security testing is performed within the controlled laboratory environment.

---

# Lab Roadmap

## Completed

* [x] Multi-OS VirtualBox Environment
* [x] Host-Only Networking
* [x] Network Troubleshooting
* [x] SSH Administration
* [x] Nmap Network Discovery
* [x] Wireshark Traffic Analysis
* [x] Linux Permissions
* [x] UFW Firewall Configuration
* [x] Apache Web Server

## In Progress

* [ ] Command Injection
* [ ] Honeypot
* [ ] Linux Log Analysis
* [ ] DNS Troubleshooting
* [ ] Additional vulnerability-testing exercises

## Planned

* [ ] Metasploitable 2 Security Testing
* [ ] Active Directory Lab
* [ ] Windows Administration & Security
* [ ] Network Segmentation
* [ ] SIEM Integration
* [ ] Linux Hardening
* [ ] Incident Response Lab
* [ ] Security Monitoring
* [ ] Security Automation
* [ ] IDS / Anomaly Detection

---

# Repository Structure

```text
multi-os-network-lab/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── documentation/
│   ├── apache-web-server-lab.md
│   ├── linux-permissions-lab.md
│   ├── network-troubleshooting-log.md
│   ├── nmap-network-discovery-lab.md
│   ├── ssh-administration-lab.md
│   ├── ufw-firewall-configuration-lab.md
│   └── wireshark-traffic-analysis-lab.md
│
└── screenshots/
    ├── linux-permissions/
    ├── networking/
    ├── nmap/
    ├── ssh/
    ├── ufw/
    └── wireshark/
```

---

# Evidence

The repository contains screenshots documenting lab activities including:

* IP configuration
* Network connectivity
* SSH sessions
* Nmap scans
* Wireshark captures
* Firewall configuration
* Linux permissions
* Network troubleshooting

Additional evidence will be added as new labs are completed.

---

# Professional Development

This laboratory is part of an ongoing technical portfolio focused on building practical experience in:

* IT support
* Linux administration
* System administration
* Networking
* Cybersecurity
* Security monitoring
* Technical troubleshooting
* Automation

The environment will continue to evolve as additional technologies and security concepts are introduced.

---

# Related Projects

Additional software-development and game-development projects are maintained in separate repositories.

Planned portfolio repositories include:

* `cybersecurity-labs`
* `windows-active-directory-lab`
* `enterprise-networking-lab`
* `security-automation`
* `gameverse`
* `alphabet-adventure`
* `portfolio-website`

---

# License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
