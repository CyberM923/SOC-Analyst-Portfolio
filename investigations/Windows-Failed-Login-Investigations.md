
# Windows Incident Response: Failed Login Investigation

## Investigation Overview

**Lab:** 4 - Windows Incident Response  
**Environment:** Windows 11 Virtual Machine (SOC-WIN11)  
**Tools:** Windows Event Viewer, PowerShell, Windows Security Logs  
**Investigation Date:** November 12, 2026  
**Status:** Investigation Completed  
**Classification:** Likely Benign Authentication Activity / Security Hardening Required

## 1. Investigation Objective

Investigate repeated Windows authentication failures, determine whether the activity indicates unauthorized access, and identify security configuration weaknesses.

The investigation focused on Windows Security Event IDs 4625, 4624, and 4740.

## 2. Initial Alert Investigation

Windows Event Viewer identified 22 failed authentication events (Event ID 4625).

### Failed Login Evidence

- Event ID: 4625
- Target account: vboxuser
- Computer: SOC-WIN11
- Logon Type: 2 (Interactive)
- Source Network Address: 127.0.0.1
- Logon Process: User32
- Caller Process: svchost.exe
- Status: 0xC000006D
- Substatus: 0xC000006A

The substatus indicates an incorrect password.

Multiple failed authentication events were observed across different dates.

### Failed Login Screenshot

![Windows Failed Login Event 4625](Windows-Failed-Login.png)

## 3. Successful Login Correlation

Windows Security Event ID 4624 was investigated to determine whether the failed authentication attempts were followed by successful logins.

### Findings

- Event ID: 4624
- Account: vboxuser
- Logon Type: 2 (Interactive)
- Failed login: November 12, 2026, 12:46:13 PM
