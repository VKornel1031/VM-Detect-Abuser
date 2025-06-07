# VM Detect Abuser

![Windows](https://img.shields.io/badge/Windows-10%2F11-0078D6?logo=windows)
![License](https://img.shields.io/badge/License-GNU-green)
![Version](https://img.shields.io/badge/Version-1.0-blue)

A security utility that tricks malware into thinking it's running in a virtual machine, causing it to terminate early. This batch script creates fake VM artifacts on physical Windows machines to enhance protection against malware.

## 🚀 Features

- **Creates convincing VM artifacts**:
  - Registry keys for VMware/VirtualBox/QEMU
  - Environment variables
  - Fake driver files and directories
  - Virtual MAC addresses

- **Interactive CLI menu**:
  - Toggle protection on/off
  - Check current status
  - Easy removal of all artifacts

- **Lightweight & reversible**:
  - No actual VM software installed
  - Full cleanup option available
  - Works alongside existing security software

## 📋 Requirements

- Windows 10/11 (Admin rights required)
- No additional software needed

## 🛠️ Installation & Usage

Just install from releases page

## 🔍 How It Works
The script creates these deception layers:

Component	What It Fakes	Malware Detection Triggered
Registry Keys	VMware/VBox services and configurations	Sandbox registry checks
Environment Vars	VM software paths and hypervisor flags	Environment scanning
Driver Files	Virtual device drivers (.sys files)	Driver-based detection
MAC Addresses	VirtualBox/VMware MAC prefixes	Network adapter checks
## ⚠️ Important Notes
Not a complete antivirus solution - Use alongside security software

May interfere with actual VM software - Disable protection first

Reboot required for MAC address changes to take effect

Test first in non-critical environments

## 🤝 Contributing
Pull requests welcome! For major changes, please open an issue first.
