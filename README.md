# Enterprise-Level Active Directory Lab

## Executive Summary

While working as an IT Support Engineer, I observed that Windows endpoint administration was performed manually. Routine tasks such as applying security configurations, enforcing USB restrictions, configuring system settings, and managing user environments required individual changes on every computer. As the number of managed endpoints increased, this approach became time-consuming, difficult to maintain, and prone to configuration inconsistencies.

To evaluate a more efficient approach, I designed and implemented an Enterprise-Level Active Directory laboratory using VMware Workstation and Windows Server. The objective was to demonstrate how centralized identity management and Group Policy could reduce administrative effort, improve consistency, and provide a scalable foundation for enterprise endpoint management.

Rather than testing these concepts in a production environment, the solution was developed inside an isolated virtual lab. The environment included Active Directory Domain Services (AD DS), Domain Name System (DNS), Organizational Units (OUs), users, security groups, and Windows client systems to validate centralized authentication and policy management.

The completed lab serves as a proof of concept for replacing repetitive manual administration with centralized Windows infrastructure. It also provides the foundation for future enterprise projects including Windows Server Update Services (WSUS), Windows Event Forwarding, Sysmon deployment, PowerShell automation, and additional infrastructure services documented throughout this portfolio.

---

## Business Problem

In my workplace, Windows endpoint administration was performed manually. Tasks such as configuring security settings, restricting USB access, managing local user configurations, and applying policy changes had to be completed individually on each computer. While this approach was manageable for a small number of devices, it became increasingly inefficient as the number of endpoints grew.

Manual administration introduced several operational challenges:

- Increased time required to configure or update multiple computers.
- Higher risk of inconsistent configurations across endpoints.
- Greater chance of human error during repetitive administrative tasks.
- Difficulty enforcing organization-wide security policies.
- Limited scalability for future business growth.

Recognizing these challenges, I wanted to explore how enterprise organizations manage hundreds or thousands of Windows devices efficiently. Rather than experimenting in a production environment, I decided to build a dedicated laboratory to understand how Active Directory could centralize identity, authentication, and policy management while reducing repetitive administrative effort.
