\# Windows Defender Monitoring



\## Overview



This document explains how Microsoft Defender Antivirus events were collected and monitored by Wazuh to detect malware-related activity on the Windows endpoint.



\## Lab Environment



\- Wazuh Manager: Ubuntu Server 22.04

\- Wazuh Version: 4.12.0

\- Endpoint: Windows 10 Home

\- Virtualization Platform: VirtualBox



\## Objectives



\- Monitor Microsoft Defender events

\- Collect Windows Defender Operational logs

\- Detect malware-related activity

\- Generate security alerts in Wazuh



\## Configuration



The Wazuh Agent was configured to monitor the Microsoft-Windows-Windows Defender/Operational event log.



Microsoft Defender Real-Time Protection remained enabled throughout testing.



\## Testing



A test detection event was generated to verify that Windows Defender logs were forwarded to Wazuh.



The Wazuh Dashboard successfully received and displayed the generated security event.



\## Detection Results



Wazuh successfully detected:



\- Microsoft Defender security events

\- Malware detection alerts

\- Antivirus operational logs

\- Endpoint protection events



\## Skills Demonstrated



\- Endpoint Security Monitoring

\- Microsoft Defender Integration

\- Windows Event Log Analysis

\- Security Alert Investigation

\- Wazuh SIEM



\## Result



Windows Defender monitoring was successfully configured and validated. Wazuh collected Microsoft Defender security events in real time, providing centralized visibility into endpoint protection activity.

