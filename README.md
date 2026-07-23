# Enterprise-Level Active Directory Lab

> A proof-of-concept enterprise Windows infrastructure demonstrating centralized identity management, authentication, and Group Policy using Windows Server 2025 and VMware Workstation.

---

## 📖 Overview

This project demonstrates the deployment of an enterprise-style Active Directory environment designed to replace manual Windows endpoint administration with centralized identity and policy management.

The lab was built after observing that administrative tasks such as user management, security configuration, and policy changes were performed manually across multiple Windows endpoints. To understand how enterprise organizations manage these tasks efficiently, I designed and implemented an isolated Active Directory environment using Windows Server 2025, VMware Workstation, Windows 10, and Windows 11.

The project serves as the foundation for additional enterprise infrastructure projects in this portfolio, including WSUS, Windows Event Forwarding (WEF), Sysmon, PowerShell automation, and Sophos Firewall integration.

---

## 🎯 Business Problem

Managing Windows endpoints manually becomes increasingly difficult as the number of devices grows.

Common administrative challenges include:

- Manual endpoint configuration
- Inconsistent security settings
- Time-consuming policy deployment
- Repetitive administrative work
- Limited scalability

In my workplace, administrative changes were typically performed by visiting each workstation or using remote support tools such as Microsoft Quick Assist and Microsoft Teams. This project explores how Active Directory centralizes these operations and improves administrative efficiency.

---

## 💡 Solution

To address these challenges, I built an Active Directory laboratory that demonstrates:

- Centralized identity management
- Domain-based authentication
- Organizational Unit (OU) design
- Group Policy management
- Windows 10 & Windows 11 domain integration
- Enterprise-ready infrastructure foundation

---

## 🏗️ Lab Architecture

> **Architecture Diagram**
>
> *(Architecture diagram will be added here.)*

---

## 🖥️ Lab Environment

### Host System

| Component | Details |
|-----------|---------|
| Host Operating System | Ubuntu 24.04.4 LTS |
| Processor | Intel Core i5-1135G7 (11th Gen) |
| Memory | 32 GB RAM |
| Storage | 512 GB NVMe SSD |
| Virtualization Platform | VMware Workstation 17.6.4 |

---

### Virtual Machines

| Hostname | Operating System | IP Address | Purpose |
|----------|------------------|------------|---------|
| WSUS-TG01 | Windows Server 2025 | 192.168.6.129 | Active Directory, DNS, Domain Controller |
| Windows 10 Client | Windows 10 | 192.168.6.200 | Domain Joined Client |
| Windows 11 Client | Windows 11 | 192.168.6.120 | Domain Joined Client |
| Sophos Firewall | Sophos Firewall | DHCP Server | Network Security & Routing |

---

### Domain Information

| Setting | Value |
|---------|-------|
| Domain Name | crop.trinix.local |
| Directory Service | Active Directory Domain Services (AD DS) |
| DNS | Active Directory Integrated DNS |
| Authentication | Domain-Based Authentication |

---

### Group Policies Tested

- USB Device Restriction
- Hide Drives
- Disable Control Panel
- Windows Update Policy

---

### Management Tools

- Active Directory Users and Computers
- Group Policy Management
- DNS Manager
- Server Manager
- VMware Workstation

## ⚙️ Technologies Used

- Windows Server 2025
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy
- VMware Workstation
- Windows 10
- Windows 11
- Sophos Firewall
- Ubuntu Linux

---

## ✅ Features Implemented

- Windows Server deployment
- Active Directory Domain Services
- DNS configuration
- Domain Controller promotion
- Domain creation (`crop.trinix.local`)
- Organizational Units (OUs)
- User account management
- Windows 10 domain join
- Windows 11 domain join
- Group Policy testing
- USB restriction policy
- Hide Drives policy
- Disable Control Panel policy
- Windows Update policy validation

---

## 📂 Repository Structure

```text
Enterprise-Level-Active-Directory-Lab
│
├── README.md
├── docs
├── diagrams
├── screenshots
├── scripts
├── configs
└── assets
```

---

## 📚 Documentation

Detailed implementation guides are available in the **docs** folder.

- Installation Guide
- Configuration Guide
- Group Policy Guide
- Validation Guide
- Troubleshooting Guide
- Lessons Learned
- Interview Notes

---

## 📸 Screenshots

The **screenshots** folder contains evidence of the deployment, including:

- Active Directory Users and Computers
- Organizational Units
- Windows Server Manager
- Domain Join
- Group Policy
- Windows Update Management
- VMware Environment

---

## 🚀 Future Improvements

Planned enhancements include:

- Secondary Domain Controller
- Active Directory Replication
- DHCP Server
- Certificate Services (AD CS)
- Microsoft Entra ID Integration
- Advanced Group Policies
- Automated Deployment Scripts

---

## 🔗 Related Projects

This project serves as the foundation for the following repositories:

- WSUS Deployment & Client Management
- Windows Event Forwarding
- Sysmon Deployment
- Sophos XGS Firewall Deployment
- PowerShell Laptop Provisioning
- Microsoft 365 Administration
- Automated IT Asset Collection

---

## 👨‍💻 Author

**Bhagath**

IT Support Engineer | Infrastructure Enthusiast

Building enterprise infrastructure projects focused on automation, centralized management, and security.
