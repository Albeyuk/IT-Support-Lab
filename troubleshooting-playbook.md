# IT Support Lab - Troubleshooting Playbook

## Overview

This playbook provides structured troubleshooting steps for common IT support and systems administration issues within the IT Support Lab environment.

It is designed to simulate real-world service desk workflows and improve problem-solving skills for entry-level IT support and cybersecurity roles.

---

## General Troubleshooting Method

When investigating any issue, follow this structured approach:

1. Identify the problem
2. Gather information (logs, user reports, system state)
3. Establish possible causes
4. Test and isolate the issue
5. Apply a fix or workaround
6. Verify resolution
7. Document the outcome

---

## 1. User Cannot Log In

### Possible Causes
- Incorrect password
- Locked Active Directory account
- Expired password
- Network connectivity issue

### Troubleshooting Steps
- Check Active Directory user status
- Verify account is not locked or disabled
- Reset password if required
- Confirm user is on the correct domain network
- Test login again

### Resolution
Unlock account or reset password and confirm successful login.

---

## 2. Network Connectivity Issues

### Possible Causes
- DNS misconfiguration
- IP address conflict
- Network adapter failure
- Router or switch issues

### Troubleshooting Steps
- Run `ipconfig /all` (Windows) or `ifconfig` (Linux)
- Test connectivity using `ping 8.8.8.8`
- Check DNS resolution using `nslookup`
- Restart network adapter
- Verify physical network connection

### Resolution
Correct IP configuration or restart network services as required.

---

## 3. Windows Updates Failing

### Possible Causes
- Corrupted update cache
- Insufficient disk space
- Service errors (Windows Update service stopped)

### Troubleshooting Steps
- Check available disk space
- Restart Windows Update service
- Clear update cache if necessary
- Run Windows Update Troubleshooter

### Resolution
Restart updates after fixing service or storage issues.

---

## 4. Backup Job Failure

### Possible Causes
- Incorrect file path
- Permission issues
- Storage device unavailable
- Script error

### Troubleshooting Steps
- Check backup logs
- Verify destination path exists
- Confirm write permissions
- Run backup script manually

### Resolution
Fix path or permissions and rerun backup automation script.

---

## 5. Slow System Performance

### Possible Causes
- High CPU or memory usage
- Background processes
- Malware or unwanted software
- Low disk space

### Troubleshooting Steps
- Check Task Manager / system monitor
- Identify high resource processes
- Run antivirus scan (if applicable in lab)
- Clear temporary files

### Resolution
Terminate unnecessary processes and free system resources.

---

## Documentation Practice

For every issue resolved:

- Record incident ID
- Document root cause
- Record resolution steps
- Suggest preventative measures

---

## Learning Outcome

This troubleshooting playbook demonstrates:

- Structured IT support methodology
- Problem isolation and resolution skills
- System administration awareness
- Real-world service desk workflow thinking
- Preparation for SOC analyst and IT support roles

---

## Disclaimer

This document is intended for educational and portfolio use only within controlled lab environments.
