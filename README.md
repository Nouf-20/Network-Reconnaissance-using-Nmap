# Network-Reconnaissance-using-Nmap
Network Reconnaissance using Nmap Conducted network scanning and service discovery on a vulnerable machine using Nmap identified open ports running services and their versions performed operating system detection and analyzed potential vulnerabilities and utilized the Nmap Scripting Engine NSE to detect misconfigurations and security weaknesses
# 🔎 Nmap Network Reconnaissance

A cybersecurity project focused on network reconnaissance and information gathering using **Nmap** in a controlled lab environment.

---

## 📌 Project Overview

Conducted in an **authorized and controlled lab environment** using **Kali Linux** (attacker) and **Metasploitable 2** (target).

The goal was to gather information about the target system and analyze exposed services, OS details, and potential weaknesses using Nmap.

> Focuses on **reconnaissance and defensive analysis**, not exploitation.

---

## 🎯 Objectives

- Host discovery & port scanning (TCP/UDP)
- Service and version detection
- Operating system detection
- Nmap Scripting Engine (NSE) usage
- Firewall / packet filtering analysis
- MAC address spoofing demonstration

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Nmap | Network scanning and reconnaissance |
| Nmap NSE | Advanced information gathering |
| Kali Linux | Security testing environment |
| Metasploitable 2 | Intentionally vulnerable target |

---

## 🔍 Key Commands

```bash
# Host discovery
nmap -sn 192.168.1.0/24

# Port scanning
nmap -sS 192.168.1.100
nmap -sU 192.168.1.100
nmap -p- 192.168.1.100

# Service & version detection
nmap -sV 192.168.1.100

# OS detection
nmap -O 192.168.1.100

# NSE scripts
nmap -sC 192.168.1.100
nmap --script vuln 192.168.1.100

# Firewall evasion
nmap -f 192.168.1.100
nmap -D RND:5 192.168.1.100

# MAC spoofing
nmap --spoof-mac 0 192.168.1.100
```

---

## 📊 Key Findings

- Multiple outdated/vulnerable services found (FTP, Telnet, VNC)
- OS fingerprint confirmed outdated Linux kernel (2.6.x)
- Highlights the need for patching, hardening, and segmentation

---

## ⚖️ Legal Notice

Only scan networks/devices you own or have **written authorization** to test (e.g. TryHackMe, Hack The Box, Metasploitable).

---

## ✅ Conclusion

Demonstrated practical Nmap-based reconnaissance in a safe lab environment, showing how attackers gather information and why defenders must proactively close these gaps.
