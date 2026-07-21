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

---

## Business Impact

The organization manages approximately 80 Windows endpoints. Administrative changes were typically performed by physically visiting workstations or by remotely connecting to users through Microsoft Quick Assist or Microsoft Teams. Depending on the type of configuration, each system could require around 10 minutes or more, especially when troubleshooting unexpected issues or device-specific behavior.

Although individual tasks were manageable, the cumulative effort required to perform the same configuration across many endpoints significantly increased administrative workload. As the organization grows, this manual approach becomes increasingly difficult to maintain while ensuring consistent security and configuration standards.

This project demonstrates how centralized management through Active Directory can improve operational efficiency by:

- Reducing repetitive administrative work.
- Providing centralized user and computer management.
- Enforcing security policies through Group Policy.
- Improving consistency across Windows endpoints.
- Creating a scalable foundation for future enterprise growth.

While this implementation was developed as a laboratory environment, it represents a practical proof of concept for modernizing Windows infrastructure management using enterprise best practices.

---

## Proposed Solution

To address the limitations of manual Windows administration, I built a centralized Active Directory laboratory that simulates a small enterprise environment.

The project initially began as a Windows Server 2025 environment for learning Windows Server Update Services (WSUS) and understanding how Windows clients receive updates from a centralized server. As the lab evolved, I recognized that enterprise environments typically rely on Active Directory to manage users, computers, and security policies. This led to the deployment of Active Directory Domain Services (AD DS) and Domain Name System (DNS), transforming the lab into a complete identity management platform.

The solution focused on the following objectives:

- Centralize user and computer management.
- Organize resources using Organizational Units (OUs).
- Prepare the environment for Group Policy implementation.
- Validate domain authentication using Windows 10 and Windows 11 client systems.
- Establish a scalable foundation for future enterprise services such as WSUS, Windows Event Forwarding, Sysmon, and PowerShell automation.

To simulate a real business environment, Organizational Units were created to separate departments and simplify administration. This structure allows different Group Policy Objects (GPOs) to be applied to specific departments. For example, one department could be granted USB access while another department could have USB storage blocked without affecting the rest of the organization.

The completed environment demonstrates how centralized identity management provides a more scalable and maintainable approach than manually configuring individual Windows computers.
