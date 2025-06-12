# IIS Installation on Azure VM

This guide explains how to install and configure IIS (Internet Information Services) on the Azure VM.

## 🔧 Steps to Install IIS

1. Log into the VM via Remote Desktop (RDP)
2. Open **Server Manager**
3. Click **Add Roles and Features**
4. Select **Web Server (IIS)** role
5. Confirm and install

## 🔍 Verify Installation

- Open browser in the VM and access: `http://localhost`
- You should see the default IIS landing page

## 🌐 Test Public Access

- Open a browser from any machine and enter the VM's public IP
- You should see the IIS page if port 80 is open

## 💡 Optional Configurations

- Replace the default IIS `index.html` with your deployed app
- Enable Application Pools for .NET if needed

