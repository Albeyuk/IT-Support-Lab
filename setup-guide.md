# IT Support Lab - Setup Guide

## Overview

This guide explains how to set up and run the IT Support Lab environment safely for learning and testing purposes. The lab is designed to simulate real IT support and systems administration tasks, including Active Directory management, system monitoring, patching, and backup automation.

## Prerequisites

Before starting, ensure you have Windows 10/11 (recommended Pro edition) or a Windows VM, an Ubuntu Linux VM, Python 3.8+, PowerShell (built into Windows), and virtualisation software such as VirtualBox, VMware, or Hyper-V.

## Lab Environment Setup

### Windows Environment

Set up a Windows machine or VM for PowerShell scripting, system administration tasks, and optional Active Directory lab work using Windows Server. Recommended setup includes Windows 10/11 Pro and optionally Windows Server 2019 or 2022 for advanced Active Directory practice.

### Linux Environment

Set up an Ubuntu VM for network monitoring scripts, system administration practice, and security-related tasks. Recommended version is Ubuntu 20.04 or later.

### Python Setup

Check if Python is installed by running: python --version. If not installed, download it from https://www.python.org/downloads/. Install required packages using pip install requests pandas.

## Repository Setup

Clone the repository using git clone https://github.com/Albeyuk/IT-Support-Lab.git then navigate into the folder using cd IT-Support-Lab.

## Running the Scripts

Run PowerShell scripts in Windows (as Administrator if required) using .\scripts\create_users.ps1, .\scripts\patch_check.ps1, and .\scripts\backup_automation.ps1. Run Python scripts using python scripts/network_monitor.py.

## Lab Exercises

Active Directory Lab (optional): install Active Directory Domain Services on Windows Server, create a domain controller, add test users and groups, and run create_users.ps1 for bulk user creation.

Patch Management Lab: use patch_check.ps1 to check missing system updates, log patch status, and simulate compliance reporting.

Backup Automation Lab: use backup_automation.ps1 to automate file backups, store backups securely, and simulate disaster recovery processes.

Network Monitoring Lab: use network_monitor.py to monitor network connectivity, track service availability, and log downtime or failures.

## Security Notes

Only use this lab in isolated or personal environments. Do not run scripts on production systems. Follow least privilege principles and use DVWA or Kali only in local lab environments.

## Troubleshooting

If Python is not found, ensure it is installed and added to PATH. If PowerShell execution is blocked, run Set-ExecutionPolicy RemoteSigned -Scope CurrentUser.

## Learning Outcomes

By completing this lab you will gain experience in IT support workflows, systems administration tasks, automation using PowerShell and Python, network and system troubleshooting, and secure lab-based operational practices.

## Disclaimer

This project is intended for educational and portfolio demonstration purposes only. It must only be used in safe, authorised lab environments.
