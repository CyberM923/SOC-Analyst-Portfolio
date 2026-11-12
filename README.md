# SOC-Analyst-Portfolio
SOC Analyst Home Lab

Overview

CompTIA Security+ (SY0-701) — Certified

I built a Security Operations Center (SOC) home lab to practice security monitoring, endpoint investigation, event analysis, and detection engineering using free tools.


Projects and Investigations

### Lab 1: Windows Endpoint Monitoring

Deployed a Wazuh SIEM homelab, integrated Windows 11 endpoint monitoring with Sysmon, and created and validated a custom detection rule (ID 100002) to identify process-creation activity.

**[View Lab 1 Investigation Report](investigations/Lab-1-Wazuh-SIEM-Detection.md)**


### Lab 2: Jira Incident Investigation (Case OPS-1)

Investigated PowerShell process activity using Wazuh and Sysmon, analyzed supporting telemetry, and documented the findings in Jira Service Management.

[View Full Report](investigations/Jira-Incident-investigation.md)

## Lab 3: Wireshark Network Traffic Investigation


Analyzed DNS queries, TCP retransmissions, and connection resets using Wireshark to investigate network behavior and identify potential connectivity issues.

[View Wireshark Investigation](investigations/Wireshark-DNS-TCP-Investigation.md)

## Lab 4: Windows Incident Response

Investigated 22 failed Windows authentication events (Event ID 4625), correlated a subsequent successful login (Event ID 4624), and assessed account security using Windows Event Viewer and PowerShell.

**[View Full Windows Incident Response Investigation](investigations/Windows-Failed-Login-Investigations.md)**

## Lab 5: MITRE ATT&CK Threat Hunting

[View MITRE ATT&CK Threat Hunting Investigation](investigations/MITRE-ATTACK-Threat-Hunting.md)


Conducted threat hunting using Wazuh and Sysmon to investigate PowerShell execution and Windows authentication activity. Mapped observed behaviors to MITRE ATT&CK techniques T1059.001 and T1110.

Disclaimer

This project is for educational purposes and uses a controlled home lab. Investigation conclusions are based only on the evidence collected during each exercise.
