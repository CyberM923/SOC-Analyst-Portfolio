
# Lab 1: Wazuh SIEM Setup & Custom Detection Rule

## Objective

Build a functional Security Operations Center (SOC) homelab using Wazuh SIEM and a Windows 11 endpoint to collect security telemetry, monitor process execution, and develop a custom detection rule.

## Lab Environment

- SIEM Platform: Wazuh
- SIEM Server: Ubuntu Linux 24.04
- Endpoint: Windows 11 ARM64
- Endpoint Monitoring: Wazuh Agent
- Endpoint Telemetry: Sysmon
- Virtualization: VirtualBox
- Investigation Tools: Wazuh Dashboard and Windows PowerShell

## Lab Architecture

The SOC homelab consists of an Ubuntu-based Wazuh server and a Windows 11 endpoint.

The Windows endpoint runs the Wazuh agent and Sysmon to collect security-relevant events.

The Wazuh server receives and analyzes endpoint telemetry, allowing process activity and security alerts to be reviewed through the Wazuh Dashboard.

## Implementation Steps

1. Deployed the Ubuntu Linux virtual machine for the Wazuh SIEM server.
2. Installed and configured Wazuh.
3. Created a Windows 11 ARM64 virtual machine.
4. Installed and connected the Wazuh agent to the Wazuh manager.
5. Installed Sysmon to collect Windows process activity.
6. Verified that Sysmon events were visible in Wazuh.
7. Created a custom Wazuh detection rule.
8. Tested the rule using process-creation activity.
9. Reviewed the resulting alert in Wazuh.

## Custom Detection Rule

**Custom Rule ID:** 100002

**Detection Objective:** Identify Windows process-creation events collected through Sysmon.

The custom rule was configured to use a built-in Wazuh rule as its parent and identify relevant Sysmon process-creation telemetry.

This exercise demonstrated how custom detection logic can extend existing SIEM monitoring capabilities.

## Detection Testing and Validation

A Windows process-creation event was generated in the controlled homelab environment.

The resulting telemetry was forwarded from the Windows endpoint to the Wazuh server.

The Wazuh Dashboard was used to confirm that the custom rule triggered and generated an alert.

### Validation Results

- Windows endpoint telemetry was successfully collected.
- Sysmon process-creation activity was visible in Wazuh.
- Custom detection rule 100002 triggered during testing.
- The resulting alert was available for investigation.

## Evidence Collected

- Wazuh Dashboard showing endpoint telemetry.
- Sysmon process-creation event.
- Custom Wazuh detection alert associated with rule 100002.
  
### Custom Wazuh Detection Evidence

![Custom Wazuh Detection Alert](https://raw.githubusercontent.com/CyberM923/SOC-Analyst-Portfolio/main/detections/wazuh-detection.jpg)

## Findings

The homelab successfully demonstrated centralized security monitoring and custom detection-rule validation.

The exercise confirmed that endpoint process activity could be collected, analyzed, and used to generate alerts through Wazuh.

The generated alert was part of controlled lab testing and did not establish malicious activity.

## Skills Demonstrated

- SIEM deployment and configuration
- Windows endpoint monitoring
- Wazuh agent integration
- Sysmon event collection
- Windows process-creation analysis
- Custom detection engineering
- Security alert validation
- SOC investigation documentation

## Conclusion

Successfully deployed a Wazuh-based SOC homelab, integrated Windows endpoint telemetry, and validated a custom detection rule using Sysmon process-creation activity.

This lab established the monitoring and detection foundation used in subsequent security investigations.

## Disclaimer

This project was completed in a controlled educational homelab. All findings and validation results are based on observed lab activity.
