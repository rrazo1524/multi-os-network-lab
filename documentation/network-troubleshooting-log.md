# Network Troubleshooting Log

## Scenario 1: Multi-VM Network Connectivity

### Objective
Establish communication between Windows, Ubuntu, and Kali Linux virtual machines in a Host-Only network environment.

---

## Environment

| System | IP Address |
|--------|------------|
| Windows 11 | 192.168.56.106 |
| Ubuntu Linux | 192.168.56.101 |
| Kali Linux | 192.168.56.103 |

---

## Problem

Initial configuration prevented communication between Windows and Linux virtual machines due to mismatched network adapter settings.

---

## Investigation

- Verified VirtualBox network adapter settings
- Confirmed all VMs were assigned Host-Only networking (or adjusted configuration)
- Checked IP addressing across all systems
- Identified that systems were on the same subnet but had connectivity issues initially

---

## Resolution

- Ensured all virtual machines were connected to the same Host-Only network
- Verified correct IP assignment on all systems
- Tested connectivity using ICMP ping

---

## Results

| Source | Destination | Status |
|--------|-------------|--------|
| Ubuntu | Windows | Success |
| Kali | Windows | Success |
| Ubuntu | Kali | Success |
| Kali | Ubuntu | Success |

---

## Key Learnings

- Virtual machines must share the same network segment to communicate
- Host-Only networking is useful for isolated lab environments
- IP addressing consistency is critical for troubleshooting
- Systematic testing helps isolate connectivity issues

---

## Skills Demonstrated

- Network troubleshooting
- VirtualBox configuration
- TCP/IP fundamentals
- Cross-platform system integration
- IT support-style problem solving
