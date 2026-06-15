# 📧 Enterprise Linux Email Server Deployment

<p align="center">
  <img src="https://img.shields.io/badge/OS-Ubuntu%20Server%2024.04%20LTS-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" />
  <img src="https://img.shields.io/badge/Mail%20Server-Citadel%20Groupware-4B4B4B?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Admin-Webmin-0078D4?style=for-the-badge&logo=webmin&logoColor=white" />
  <img src="https://img.shields.io/badge/Firewall-UFW-E22C2C?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Platform-VMware-607078?style=for-the-badge&logo=vmware&logoColor=white" />
</p>

> 🖥️ End-to-end deployment and configuration of an enterprise email server on Ubuntu Server 24.04 LTS using Citadel Groupware — including DNS/MX record configuration, UFW firewall rules, Webmin administration, DHCP reservations, user management, and full email service testing.

---

## 📌 Overview

This project demonstrates the complete lifecycle of deploying an **enterprise-grade email infrastructure** in a virtualized environment. It simulates a real-world organizational mail system for the **ACME.EDU** domain — from initial Ubuntu Server setup through DNS configuration, mail server installation, firewall hardening, and end-to-end email testing.

**Environment:** VMware Workstation | Ubuntu Server 24.04 LTS | Domain: `ACME.EDU`

---

## 🏗️ System Architecture

```
[VMware Workstation]
        │
        ├── DNS Server (Windows Server)
        │     ├── Forward Lookup Zone: ACME.EDU
        │     ├── MX Record → AcmePCEm01.ACME.EDU
        │     ├── Host (A) Record: AcmePCEm01 → 192.168.4.35
        │     └── PTR Record (Reverse Lookup)
        │
        └── Ubuntu Email Server (AcmePCEm01)
              ├── Static IP: 192.168.4.35
              ├── Webmin → Port 10000
              ├── Citadel Mail Server
              │     ├── SMTP → Port 25
              │     ├── HTTP → Port 80
              │     ├── HTTPS → Port 443
              │     └── Citadel → Port 504
              └── UFW Firewall
```

---

## 🛠️ Technologies Implemented

### 🐧 Server & OS
- **Ubuntu Server 24.04 LTS** — base OS with static IP configuration
- **VMware Workstation** — virtualization platform

### 📬 Email Services
- **Citadel Groupware Server** — full-featured enterprise mail server (SMTP, IMAP, webmail)
- **WebCit** — Citadel's web-based mail client interface
- **Usermin** — user-level web-based mail access

### 🌐 Network Services
- **DNS** — forward/reverse lookup zones, MX records, PTR/CNAME/A records
- **DHCP Reservation** — static IP assignment for email server (`192.168.4.35`)
- **UFW Firewall** — port-based access control

### ⚙️ Administration
- **Webmin** — web-based Linux server administration (Port 10000)
- **Bash/CLI** — package installation, service configuration, network setup

---

## 📋 Implementation Steps

| Step | Task | Details |
|------|------|---------|
| 1 | DNS Configuration | Forward/reverse zones, MX record, A/PTR/CNAME records |
| 2 | Ubuntu Server Setup | Static IP, DNS settings, gateway, root access |
| 3 | Webmin Installation | Web-based admin portal on port 10000 |
| 4 | Usermin Installation | User-level web mail access |
| 5 | Citadel Installation | Full mail server with SMTP, webmail, auth |
| 6 | UFW Firewall Rules | Allow SSH, SMTP, HTTP, HTTPS, Citadel, Webmin |
| 7 | DHCP Reservation | Static address binding for email server |
| 8 | User Account Creation | Multiple mailbox users created and tested |
| 9 | Email Testing | Transmission, delivery, reply, and webmail verification |

---

## 🔒 Firewall Configuration

| Service | Port | Protocol | Status |
|---------|------|----------|--------|
| SSH | 22 | TCP | ✅ Allowed |
| SMTP | 25 | TCP | ✅ Allowed |
| HTTP | 80 | TCP | ✅ Allowed |
| HTTPS | 443 | TCP | ✅ Allowed |
| Citadel | 504 | TCP | ✅ Allowed |
| Webmin | 10000 | TCP | ✅ Allowed |

---

## 👥 User Accounts Created & Tested

| Username | Role |
|----------|------|
| MMcMann | Staff |
| CWilkers | Staff |
| CChristi | Staff |
| JAwsome | Staff |
| SecTest | Security Testing |
| HKodippilige | Administrator |

---

## ✅ Testing & Verification

- ✅ Email transmission between internal users verified
- ✅ Mailbox delivery confirmed via WebCit webmail
- ✅ Reply and forwarding functionality tested
- ✅ Webmin admin portal accessible on port 10000
- ✅ Usermin accessible for end-user mailbox management
- ✅ DNS MX record resolution verified
- ✅ Firewall rules confirmed — only required ports open

---

## 📁 Repository Contents

```
📦 Linux-email-server-deployment
├── 📄 README.md
└── 📋 E-mail Server Installation and Setup instructions-KHS.pdf
```

---

## 🧠 Skills Demonstrated

`Ubuntu Server` `Linux Administration` `Citadel Groupware` `Webmin` `DNS Configuration` `MX Records` `UFW Firewall` `DHCP Reservations` `Email Infrastructure` `SMTP` `User Management` `VMware` `Network Services` `System Administration`

---

## 💡 Real-World Relevance

Enterprise email infrastructure is a core component of organizational IT. This project demonstrates skills applicable to:
- **Linux System Administrator** roles — Ubuntu server deployment, service configuration
- **IT Infrastructure Engineer** roles — DNS, DHCP, firewall, mail server setup
- **Security Engineer** roles — firewall hardening, secure service configuration
- **PhD Research** — server-side security configuration, protocol analysis environments

---

## ⚠️ Disclaimer

This project was deployed in a controlled VMware virtualization environment for academic and educational purposes. All domain names, usernames, and IP addresses are fictitious.

---

## 👤 Author

**Hashan Kodippilige**  
M.S. Cybersecurity — Minnesota State University Moorhead  
📧 hashansharindu@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/hashankodippilige/)  
🐙 [GitHub](https://github.com/hashan-kodippilige)
