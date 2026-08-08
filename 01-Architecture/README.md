# Enterprise Architecture & Planning

## Project Overview

This project simulates the design, deployment, administration, and support of a small enterprise IT environment. The environment integrates on-premises Active Directory with Microsoft Entra ID, Microsoft 365, Intune, PowerShell, Windows Server, and ServiceNow.

## Organization

**Company:** Contoso Enterprise
**Employees:** Approximately 75
**Environment:** Hybrid on-premises and cloud

### Departments

* IT
* Human Resources
* Finance
* Sales
* Marketing
* Operations
* Management

## Planned Infrastructure

| System   | Role                                   | Operating System |
| -------- | -------------------------------------- | ---------------- |
| DC01     | Active Directory Domain Services + DNS | Windows Server   |
| SRV01    | File Server + DHCP                     | Windows Server   |
| WIN11-01 | Employee Workstation                   | Windows 11       |
| WIN11-02 | Employee Workstation                   | Windows 11       |

## Network Plan

**Network:** 192.168.10.0/24
**Gateway:** 192.168.10.1
**DC01:** 192.168.10.10
**SRV01:** 192.168.10.20
**DHCP Range:** 192.168.10.100–192.168.10.200

## Active Directory

**Domain:** corp.contoso.local

### Organizational Units

```text
corp.contoso.local
│
├── Users
│   ├── IT
│   ├── HR
│   ├── Finance
│   ├── Sales
│   ├── Marketing
│   ├── Operations
│   └── Management
│
├── Computers
│   ├── Workstations
│   └── Laptops
│
├── Servers
│
└── Groups
```

## Security Groups

* GG-IT
* GG-HR
* GG-Finance
* GG-Sales
* GG-Marketing
* GG-Operations
* GG-Management

## Naming Conventions

### Users

`firstname.lastname`

Example:

`john.smith`

### Computers

`WIN11-01`
`WIN11-02`

### Servers

`DC01`
`SRV01`

### Security Groups

`GG-Department`

Example:

`GG-IT`

## Planned Technologies

* Windows Server
* Active Directory
* DNS
* DHCP
* Group Policy
* PowerShell
* Microsoft Entra ID
* Microsoft 365
* Microsoft Intune
* ServiceNow

## Project Goal

The goal is to build and document a realistic enterprise IT environment that demonstrates identity management, endpoint administration, automation, troubleshooting, security controls, user lifecycle management, and IT service management.
