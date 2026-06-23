# SSH Administration Lab

## Objective

Configure and test Secure Shell (SSH) remote administration between Kali Linux and Ubuntu Linux virtual machines within a VirtualBox home lab environment.

---

## Environment

| System | Role | IP Address |
|----------|----------|----------|
| Ubuntu Linux | SSH Server | 192.168.56.101 |
| Kali Linux | SSH Client | 192.168.56.104 |

---

## Technologies Used

- Ubuntu Linux
- Kali Linux
- OpenSSH Server
- OpenSSH Client
- VirtualBox
- TCP/IP Networking
- Linux Command Line

---

## Lab Overview

This lab demonstrates the configuration and use of SSH (Secure Shell) for remote administration. SSH provides encrypted remote access to systems and is commonly used by system administrators, cloud engineers, and cybersecurity professionals.

The objective was to configure Ubuntu as an SSH server and establish a remote connection from Kali Linux.

---

## Installation and Configuration

### Update Package Repository

```bash
sudo apt update
```

### Install OpenSSH Server

```bash
sudo apt install openssh-server -y
```

### Verify SSH Service

```bash
sudo systemctl status ssh
```

### Verify SSH Listening Port

```bash
sudo ss -tlnp | grep :22
```

Results confirmed that the SSH service was running and listening on TCP port 22.

---

## Connectivity Testing

Prior to SSH testing, network communication was verified between Kali Linux and Ubuntu Linux.

### Ping Test

```bash
ping 192.168.56.101
```

Successful responses confirmed connectivity between both systems on the Host-Only network.

---

## Remote Access

### SSH Connection

From Kali Linux:

```bash
ssh username@192.168.56.101
```

The SSH client prompted for authentication using the Ubuntu user account password.

After successful authentication, a remote shell session was established on the Ubuntu system.

---

## Administrative Commands Executed

The following commands were executed remotely through the SSH session:

### Verify Logged-In User

```bash
whoami
```

### Display Hostname

```bash
hostname
```

### Display System Information

```bash
uname -a
```

### Display Current Directory

```bash
pwd
```

### List Directory Contents

```bash
ls -la
```

### Display User Information

```bash
id
```

---

## Troubleshooting

### Issue 1: SSH Service Not Running

The SSH service was initially inactive after installation.

Resolution:

```bash
sudo systemctl start ssh
sudo systemctl enable ssh
```

---

### Issue 2: Network Connectivity Problems

SSH connections initially failed due to VirtualBox network adapter configuration issues.

Resolution:

- Verified Host-Only adapter settings
- Confirmed Ubuntu and Kali were on the same subnet
- Validated connectivity using ICMP ping tests

---

### Issue 3: Authentication Failure

SSH authentication initially failed because an incorrect username was used during login attempts.

Resolution:

- Verified the active Ubuntu username using:

```bash
whoami
```

- Reconnected using the correct username

Authentication then succeeded.

---

## Results

| Test | Result |
|--------|--------|
| SSH Server Installation | Success |
| SSH Service Running | Success |
| Port 22 Listening | Success |
| Kali to Ubuntu Connectivity | Success |
| Remote Authentication | Success |
| Remote Command Execution | Success |

---

## Skills Demonstrated

- Linux Administration
- SSH Configuration
- Remote System Administration
- Network Troubleshooting
- VirtualBox Networking
- Command Line Operations
- TCP/IP Networking
- User Authentication
- Technical Documentation

---

## Evidence

Screenshots stored in:

```text
screenshots/ssh/
```

Suggested screenshots:

- ssh-login-success.png
- whoami-output.png
- hostname-output.png
- uname-output.png

---

## Real-World Relevance

SSH is one of the most widely used tools in information technology, cloud computing, and cybersecurity. System administrators use SSH to remotely manage servers, troubleshoot issues, perform maintenance, and securely administer systems across networks.

This lab demonstrates practical experience configuring remote access, validating connectivity, troubleshooting authentication issues, and managing Linux systems through a secure command-line interface.

---

## Conclusion

This lab provided hands-on experience configuring and using SSH in a multi-operating system virtual environment. By successfully establishing secure remote access between Kali Linux and Ubuntu Linux, the lab strengthened skills in Linux administration, networking, troubleshooting, and remote system management.
