# Azure DevOps Agent Installation on VM

This file covers how to install a self-hosted agent on the Azure VM and register it to a Deployment Group.

## 🔗 Steps

1. In Azure DevOps > **Pipelines > Deployment Groups**
2. Create a new Deployment Group (e.g., "IIS-Prod-VM")
3. Generate the **PowerShell registration script** (it contains a token and download URL)
4. Run the script inside the VM using PowerShell and it will create an agent
