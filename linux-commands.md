# Linux Commands For Beginners 

## 1. Introduction 
Linux is an operating system widely used in servers and cloud computing .

## 2. Basics Linux Commands 

### pwd
Shows the current working directory.
### ls
Lists Files and folders.

### cd
Changes the current directory
### mkdir
Creates a new directory

### whoami
Shows the current username .

### 3. Learning Goal
I am learning Linux basics to build my knowledge of Cyber Security and Cloud Security .
### cd ~
Moves to the current user's home directory
### ls -a
Lists all files and folders, including hidden ones.
## DNS (Domain Name System)

DNS converts domain names into IP addresses.

Example:
- `google.com`
- `youtube.com`

### DNS Command

```bash
nslookup google.com
```

### Purpose
The `nslookup` command is used to find the IP addresses associated with a domain name.

### Important Points
- Chrome automatically performs DNS resolution when opening websites.
- We use `nslookup` to manually check DNS information.
- A domain can return multiple IP addresses.

### What I Learned
DNS helps computers locate websites using their domain names.
## Ports and Protocols

A port is a number used to identify a specific service or application on a computer.

### Important Network Ports

| Port | Protocol/Service | Purpose |
|---|---|---|
| 22 | SSH | Secure remote login |
| 53 | DNS | Domain name resolution |
| 80 | HTTP | Web communication |
| 443 | HTTPS | Secure web communication |

### TCP vs UDP

**TCP:**
- Reliable data delivery.
- Uses acknowledgements and retransmission.
- Example: SSH and many file transfers.

**UDP:**
- Does not guarantee delivery.
- Lower communication overhead.
- Example: Online gaming and live calls.

### Practical Command

```bash
ss -tuln
```

Purpose: Displays listening TCP and UDP sockets with numeric addresses and port numbers.
## Firewall and UFW

A firewall controls incoming and outgoing network traffic based on security rules.

### UFW
UFW stands for Uncomplicated Firewall. It is a firewall management tool available on Ubuntu.

### Commands

```bash
sudo apt install ufw -y
sudo ufw status
```

### Important Firewall Rules

- Allow 22: Allow SSH traffic.
- Allow 80: Allow HTTP traffic.
- Allow 443: Allow HTTPS traffic.

### Learning
- Allow means permit network traffic.
- Deny means block network traffic.
- In my Ubuntu WSL environment, UFW is installed but currently inactive.
