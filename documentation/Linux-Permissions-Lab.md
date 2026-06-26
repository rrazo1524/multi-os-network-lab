# 🐧 Linux Permissions Lab

## Objective

The objective of this lab was to configure and validate Linux file permissions using users, groups, and shared directories. This lab demonstrates how Linux enforces access control through ownership and permission bits, and how group membership enables secure collaboration between multiple users in a shared environment.

---

## Lab Environment

This lab was conducted in an Ubuntu Linux virtual machine running inside VirtualBox with a Host-Only network configuration.

| User | Role |
|------|------|
| alice | Standard user |
| lucifer151 | Standard user |
| root | System administrator |

| Group | Purpose |
|-------|--------|
| projectteam | Shared collaboration group |

---

## Technologies Used

- Ubuntu Linux
- Bash shell
- User management tools (`useradd`, `usermod`)
- Group management (`groupadd`)
- File and directory permissions (`chmod`, `chown`)
- Linux access control model

---

## Methodology

1. Create a shared group for controlled access
2. Create a secured shared directory
3. Configure ownership and permissions
4. Add users to the group
5. Test file creation and access between users
6. Verify permission behavior and troubleshoot issues

---

## Step 1: Create Group

```bash
sudo groupadd projectteam

```
## Step 2: Create Shared Directory

```bash
sudo mkdir /projectlab

```
## Step 3: Configure Ownership and Permissions

```bash
sudo chowm root:projecctteam /projectlab
sudo chmod 770 /projectlab

```


