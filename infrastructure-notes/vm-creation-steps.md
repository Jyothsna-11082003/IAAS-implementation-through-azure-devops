# Azure VM Creation Steps

This document outlines the steps to create a Windows Virtual Machine in Azure for deploying a web application using IIS.

## 🧱 VM Configuration

- **Azure Portal > Virtual Machines > Create**
- **OS**: Windows Server 2019 or 2022
- **Size**: Standard B1s or above (depending on app load)
- **Authentication**: Password-based
- **Inbound Ports**: HTTP (80), RDP (3389)

## 🔐 Networking

- **Public IP**: Enabled (for accessing IIS web page)
- **NSG Rules**: Allowed inbound traffic on port 80 (HTTP) and port 3389 (RDP)

## 🛠 Post-Creation Steps

1. **Connect to VM** using RDP with the assigned public IP
2. **Update Windows**
3. **Install Required Tools**:
   - Web Server (IIS)
   - Git (optional)
   - Azure DevOps agent dependencies (PowerShell, .NET)

