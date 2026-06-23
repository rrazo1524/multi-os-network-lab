# Network Troubleshooting Log

## Scenario: Multi-VM Network Connectivity

### Objective

Establish communication between Windows, Ubuntu, and Kali Linux virtual machines in a Host-Only network environment.

---

## Environment

| System | IP Address |
|--------|------------|
| Windows 11 | 192.168.56.106 |
| Ubuntu Linux | 192.168.56.101 |
| Kali Linux | 192.168.56.104 |

---

## Problem

Initial configuration prevented communication between Windows and Linux virtual machines due to inconsistent VirtualBox network adapter settings. Although systems were assigned IP addresses within the same subnet (192.168.56.0/24), ICMP traffic (ping) initially failed between hosts.

---

## Investigation

- Reviewed VirtualBox network adapter configurations across all virtual machines to ensure consistent Host-Only networking.
- Confirmed Host-Only networking was enabled
- Checked IP addressing on Windows, Ubuntu, and Kali Linux
- Verified all systems were within the same subnet (192.168.56.0/24)
- Performed initial connectivity testing using ICMP (ping)

---

## Resolution

- Standardized all virtual machines to use the same Host-Only network adapter
- Verified correct IP assignment across all systems
- Restarted network interfaces on affected virtual machines to apply configuration changes
- Re-tested connectivity using ICMP (ping)

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

## Real-World Relevance

This scenario simulates a common IT support issue where systems appear correctly configured but fail to communicate due to network misalignment. The troubleshooting process mirrors real-world tasks performed in help desk and system administration roles.

## Conclusion

This exercise reinforced foundational networking concepts and provided hands-on experience troubleshooting virtualized environments commonly used in IT support and system administration roles.
