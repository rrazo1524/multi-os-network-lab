# Wireshark Traffic Analysis Lab

## Objective

The objective of this lab was to capture and analyze live network traffic in a multi-VM environment using Wireshark. The focus is on understanding TCP/IP communication, identifying protocols, and observing encrypted vs unencrypted traffic.

---

## Lab Environment

All virtual machines are connected using a VirtualBox Host-Only network.

| System | Role | IP Address |
|--------|------|------------|
| Windows 11 | Traffic Generation / Client | 192.168.56.106 |
| Ubuntu Linux | SSH Server | 192.168.56.101 |
| Kali Linux | Packet Analysis Tool | 192.168.56.104 |

---

## Tools Used

- Wireshark
- VirtualBox
- Kali Linux
- Ubuntu Linux
- Windows 11
- SSH (OpenSSH Server)
- Nmap (traffic generation)

---

## Methodology

The following steps were performed:

1. Start Wireshark capture on Kali Linux (eth0)
2. Generate network traffic using ping, SSH, and Nmap
3. Capture and analyze packets in real time
4. Filter traffic using Wireshark display filters
5. Identify TCP handshake, ICMP, and encrypted SSH traffic

---

## Step 1: Start Capture

### Command (Wireshark GUI)
Select interface:
- `eth0` (Host-Only adapter)

Click:
- ▶ Start Capture

---

## Step 2: Generate ICMP Traffic (Ping Test)

### Command (Windows or Kali or Ubuntu)

```bash
ping 192.168.56.101
```

### Wireshark Filter

```text
icmp
```

### Observed Results

- ICMP Echo Request packets were captured.
- ICMP Echo Reply packets confirmed successful communication.

---

## Step 3: Generate SSH Traffic

### Command (Kali → Ubuntu)

```bash
ssh lucifer151@192.168.56.101
```

### Wireshark Filter

```text
tcp.port == 22
```

### Observed Results

- TCP three-way handshake was observed.
- SSH packets were visible on port 22.
- User commands and responses were encrypted after authentication.

---

## Step 4: Generate Nmap Scan Traffic

### Command (Kali)

```bash
nmap -n -T4 -F 192.168.56.101
```

### Wireshark Filter

```text
tcp.flags.syn == 1
```

### Observed Results

- Multiple TCP SYN packets were captured during the Nmap scan.
- Responses from the Ubuntu SSH service confirmed port discovery activity.

---

## Step 5: General Traffic Overview

### Wireshark Filter

```text
tcp
```

### Observations
- TCP handshake patterns
- Repeated retransmissions (if any)
- Mixed traffic from SSH and scanning tools

---

## Evidence

### Wireshark Capture Overview

![Wireshark Main Interface](../screenshots/wireshark/wireshark-main.png)

### ICMP Traffic Analysis

![ICMP Traffic](../screenshots/wireshark/icmp-traffic.png)

### SSH Traffic Analysis

![SSH Traffic](../screenshots/wireshark/ssh-traffic.png)

### Nmap Scan Traffic

![Nmap Traffic](../screenshots/wireshark/nmap-traffic.png)


---

## Key Findings

- ICMP traffic is unencrypted and clearly visible in packet captures
- SSH traffic is encrypted after handshake (payload not readable)
- Nmap scans generate identifiable SYN scan patterns
- TCP/IP communication follows predictable handshake behavior
- Network traffic can be filtered and analyzed in real time using Wireshark

---

## Security Observations

- SSH encryption protects data payload from inspection
- ICMP traffic can be used for network reconnaissance
- Port scanning activity is detectable via SYN patterns
- Network monitoring tools can identify suspicious behavior

---

## Real-World Relevance

Wireshark is widely used in:

- Cybersecurity incident response
- Network troubleshooting
- Packet-level analysis
- Malware investigation
- SOC (Security Operations Center) monitoring

This lab demonstrates foundational packet analysis skills used by network engineers and security analysts.

---

## Skills Demonstrated

- Packet capture and analysis
- TCP/IP protocol understanding
- Network troubleshooting
- Traffic filtering using display filters
- Security monitoring fundamentals
- SSH and encrypted traffic analysis

---

## Conclusion

This lab successfully demonstrated how to capture and analyze network traffic using Wireshark. Key protocols such as ICMP, TCP, and SSH were observed and analyzed. The exercise provided foundational skills in packet analysis and network security monitoring.

---
