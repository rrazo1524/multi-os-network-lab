## Outcome

After configuring a Host-Only network adapter for the Windows virtual machine and validating IP addressing across all systems, successful communication was established between Windows, Ubuntu, and Kali Linux.

### Connectivity Validation

| Source | Destination | Result |
|----------|----------|----------|
| Ubuntu | Windows | Success |
| Kali Linux | Windows | Success |
| Ubuntu | Kali Linux | Success |
| Kali Linux | Ubuntu | Success |

### Lessons Learned

- Virtual machines must share the same network segment to communicate.
- Host-Only networking provides an isolated environment for lab testing.
- IP configuration and network adapter settings should be verified before troubleshooting higher-layer services.
- Cross-platform connectivity testing is an effective method for diagnosing network issues.
