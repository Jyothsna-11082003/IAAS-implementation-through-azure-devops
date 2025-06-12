# Release Pipeline Details

This file describes the configuration of the Azure DevOps Release Pipeline that deploys the build artifact to a VM using IIS.

## 🚀 Pipeline Setup

1. **Stage**: Deploy to IIS
2. **Environment**: Connected via a Deployment Group targeting the Azure VM
3. **Tasks Used**:
   - **IIS Web App Deployment**
     - Package or folder: Pointed to the published build artifact directory (`WebPublish`)
     - Deployment group: The VM where the agent is installed
     - Website name: Example - "Default Web Site" or custom

## 🔐 VM Configuration

- IIS is manually installed on the VM.
- Agent script was run to register the VM with the deployment group.


## ✅ Outcome

- The web application is deployed successfully and accessible via the public IP of the VM.
