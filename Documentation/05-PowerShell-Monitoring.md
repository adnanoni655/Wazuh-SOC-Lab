\# PowerShell Monitoring



\## Overview



This document explains how PowerShell activity was monitored using Wazuh to detect potentially suspicious script execution on the Windows endpoint.



\## Lab Environment



\- Wazuh Manager: Ubuntu Server 22.04

\- Wazuh Version: 4.12.0

\- Endpoint: Windows 10 Home

\- Virtualization Platform: VirtualBox



\## Objectives



\- Enable PowerShell event logging

\- Collect PowerShell Operational logs

\- Detect PowerShell command execution

\- Map alerts to the MITRE ATT\&CK framework



\## Configuration



PowerShell Operational Logging and Script Block Logging were enabled on the Windows endpoint.



The Wazuh Agent was configured to monitor the Microsoft-Windows-PowerShell/Operational event log.



\## Testing



A PowerShell command was executed on the endpoint to generate security events.



Wazuh collected the logs and generated alerts within the dashboard.



\## Detection Results



Wazuh successfully detected:



\- PowerShell execution

\- Script execution events

\- Registry modification activity

\- Security alerts mapped to MITRE ATT\&CK



\## MITRE ATT\&CK Mapping



\- T1059.001 – PowerShell

\- T1112 – Modify Registry



\## Skills Demonstrated



\- Windows Event Monitoring

\- PowerShell Logging

\- Security Event Analysis

\- Threat Detection

\- MITRE ATT\&CK Mapping

\- Wazuh SIEM



\## Result



PowerShell monitoring was successfully configured and validated. Wazuh detected PowerShell execution events in real time and mapped the activity to the MITRE ATT\&CK framework, demonstrating effective endpoint monitoring and threat detection capabilities.

