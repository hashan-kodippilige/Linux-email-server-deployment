# Linux Email Server Deployment

## Overview

This project demonstrates the complete deployment and configuration of an enterprise email server using Ubuntu Server, Citadel Groupware, and Webmin.

The environment includes DNS configuration, DHCP reservations, firewall management, mail server deployment, web-based administration, user account creation, and email service testing.

The project was completed in a virtualized environment and simulates a real-world organizational email infrastructure.

---

## Project Objectives

- Deploy Ubuntu Server
- Configure DNS services
- Create mail exchange (MX) records
- Install and configure Webmin
- Deploy Citadel Email Server
- Configure firewall security rules
- Create user accounts
- Test email communication
- Verify mail delivery and messaging functionality

---

## Technologies Used

### Operating System
- Ubuntu Server 24.04 LTS

### Administration Tools
- Webmin
- Usermin

### Email Services
- Citadel Groupware Server
- WebCit Web Interface

### Networking Services
- DNS
- DHCP
- Firewall (UFW)

### Virtualization
- VMware Workstation

---

## Key Skills Demonstrated

✔ Linux Server Administration

✔ Ubuntu Server Deployment

✔ DNS Configuration

✔ MX Record Configuration

✔ DHCP Reservations

✔ Webmin Administration

✔ Citadel Mail Server Deployment

✔ Firewall Management

✔ User Account Administration

✔ Email Infrastructure Management

✔ Network Services Configuration

✔ System Troubleshooting

---

## Project Architecture

### Domain Structure

```text
ACME.EDU
│
├── DNS Server
│
├── MX Record
│   └── AcmePCEm01.ACME.EDU
│
├── Email Server
│   └── Ubuntu Server 24.04
│
├── Webmin Management
│   └── Port 10000
│
└── Citadel Mail Services
    ├── SMTP (25)
    ├── HTTP (80)
    ├── HTTPS (443)
    └── Citadel Service (504)
```

---

## Project Tasks

### 1. DNS Configuration

Configured:

- Forward Lookup Zones
- Reverse Lookup Zones
- Host Records
- MX Records
- PTR Records
- CNAME Records

### 2. Ubuntu Server Installation

Configured:

- Static IP Addressing
- DNS Settings
- Gateway Configuration
- Root Account Access

### 3. Webmin Deployment

Installed and configured:

- Webmin
- Usermin
- Remote Web Administration

### 4. Citadel Mail Server Installation

Configured:

- SMTP Services
- WebMail Access
- Authentication Settings
- User Mailboxes

### 5. Firewall Configuration

Allowed services:

| Service | Port |
|----------|------|
| SSH | 22 |
| SMTP | 25 |
| HTTP | 80 |
| HTTPS | 443 |
| Citadel | 504 |
| Webmin | 10000 |

### 6. DHCP Reservation

Created DHCP reservation for:

```text
192.168.4.35
```

### 7. User Management

Created multiple user accounts including:

- MMcMann
- CWilkers
- CChristi
- JAwsome
- SecTest
- HKodippilige

### 8. Testing

Performed:

- Email transmission testing
- Mailbox verification
- Reply testing
- Internal messaging validation
- Webmail access testing

---

## Learning Outcomes

Through this project I gained experience in:

- Enterprise Email Infrastructure
- Linux Server Administration
- DNS and Mail Routing
- Firewall Security Configuration
- Web-Based Server Administration
- Virtualized Infrastructure Deployment
- User Account Management
- Email System Testing

---

## Repository Structure

```text
README.md

Email-Server-Installation.pdf

screenshots/
configuration-files/
network-diagrams/
```

---

## Author

Hashan Kodippilige
Master of Science in Cybersecurity
Minnesota State University Moorhead

Cybersecurity | Linux Administration | Splunk | System Administration | Network Security
