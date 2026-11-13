# SOC Analyst | Cybersecurity Portfolio

I'm an aspiring SOC Analyst with a **CompTIA Security+ certification** and a **Google Cybersecurity Professional Certificate**, complemented by hands-on experience in security monitoring, threat detection, incident response, and network traffic analysis.

Through eight practical cybersecurity labs, I've developed experience investigating security alerts, analyzing logs, identifying suspicious activity, and documenting security incidents using industry-standard tools.

## Certifications
- CompTIA Security+
- Google Cybersecurity Professional Certificate — Coursera

## Core Technical Skills

- **SIEM & Endpoint Security:** Wazuh, Sysmon, SIEM monitoring, security alert triage, custom Wazuh detection rules, detection rule testing and tuning
- **Threat Detection & Hunting:** MITRE ATT&CK, IOC investigation, PowerShell investigation, suspicious process analysis, security event correlation
- **Incident Response:** Windows Event Viewer, Windows authentication analysis, failed and successful login investigations, incident classification, false-positive analysis, escalation procedures
- **Network Security:** Wireshark, Zeek, Suricata IDS, DNS analysis, TCP traffic analysis, packet inspection, network intrusion detection
- **Security Analytics:** Kusto Query Language (KQL), Microsoft Azure Logs Demo, authentication log analysis, security event filtering
- **Ticketing & Reporting:** Jira Service Management, incident documentation, investigation reports, SOC shift handoffs
- **Operating Systems:** Windows 11, Ubuntu Linux, Linux command line, PowerShell
- **Virtualization & Homelabs:** Oracle VirtualBox, virtual machine configuration, Windows and Linux security lab environments


## Career Goal

Seeking an entry-level remote SOC Analyst opportunity where I can apply my technical skills, cybersecurity certifications, and practical security investigation experience.


## Projects and Investigations

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


### Lab 6: Suricata IDS + Zeek Network Monitoring


Deployed Suricata IDS and Zeek 9.0.1 in a virtual cybersecurity homelab to monitor network traffic, create custom detection rules, and investigate network activity.


**Investigation Reports:**


- [Suricata IDS Investigation](investigations/Suricata-IDS/Suricata-IDS-Investigation.md)
- [Zeek Network Monitoring Investigation](investigations/Zeek-Network-Monitoring/Zeek-Network-Investigation.md)


### Lab 7: KQL Authentication Investigation

Conducted a simulated security investigation using Kusto Query Language (KQL) in Microsoft's Azure Logs demo environment.


**Investigation Report:**

[KQL Authentication Investigation](investigations/KQL-Authentication-Investigations/README.md)


### Lab 8: SOC Shift Simulation

Investigated high-severity Wazuh alerts, analyzed Sysmon process activity, identified likely false positives, and documented findings using SOC incident response procedures.

[View Lab 8 Investigation](investigations/SOC-Shift-Simulation/README.md)








Disclaimer

This project is for educational purposes and uses a controlled home lab. Investigation conclusions are based only on the evidence collected during each exercise.
