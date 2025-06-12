# 🚀 Azure DevOps IIS Deployment (IaaS Implementation)

This project demonstrates an end-to-end CI/CD pipeline using Azure DevOps to deploy a .NET web application onto a Virtual Machine (VM) in Azure, where IIS (Internet Information Services) is used as the web server.

> 🔒 **Note:** Organization name has been hidden for privacy purposes.

---

## 📌 Project Overview

- 👩‍💻 Created a deployment pipeline using Azure DevOps
- 🏗️ Built and published a .NET application using NuGet and MSBuild tasks
- 📦 Packaged artifacts as `.dll` files
- 🖥️ Deployed the app onto an Azure VM using a self-hosted agent
- 🌐 Configured IIS on the VM to host the deployed web app

---

## 🧰 Technologies & Tools Used

- Azure DevOps (Pipelines, Deployment Groups)
- Azure Virtual Machine (Windows Server)
- IIS (Internet Information Services)
- .NET Framework
- Git + GitHub
- PowerShell (for agent registration)
- Markdown for documentation

---

## 🏗️ Architecture

```text
+----------------------+         +---------------------------+
|  Azure DevOps        |  CI/CD  |   Azure VM (Windows)      |
|  ------------------  |-------> |   - IIS Enabled           |
|  - Pipeline Tasks     |        |   - Self-hosted agent     |
|  - Artifacts (.dll)   |        |   - Web App Hosted        |
+----------------------+         +---------------------------+
