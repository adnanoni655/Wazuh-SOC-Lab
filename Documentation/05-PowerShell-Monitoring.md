# PowerShell Monitoring

## Overview

This document explains how I configured Wazuh to monitor PowerShell activity on a Windows 10 endpoint. By enabling PowerShell Operational Logging and Script Block Logging, Wazuh was able to detect PowerShell execution and map events to the MITRE ATT&CK framework.

## Lab Environment

- **Manager:** Wazuh 4.12.0
- **Operating System:** Ubuntu Server 22.04 LTS
- **Endpoint:** Windows 10 Home
- **Virtualization Platform:** VirtualBox

## Objectives

- Enable PowerShell Operational Logging
- Enable Script Block Logging
- Monitor PowerShell execution
- Verify detection in the Wazuh Dashboard
- Map alerts to MITRE ATT&CK

## Steps Performed

1. Enabled PowerShell Operational Logging.
2. Enabled PowerShell Script Block Logging.
3. Executed PowerShell commands on the Windows endpoint.
4. Allowed the Wazuh Agent to collect PowerShell events.
5. Verified alerts in the Wazuh Dashboard.
6. Reviewed the associated MITRE ATT&CK techniques.

## Detection Results

Wazuh successfully detected PowerShell execution and generated security alerts. The alerts were mapped to the MITRE ATT&CK framework, demonstrating how PowerShell activity can be monitored and analyzed for suspicious behavior.

Example detection:

- **Rule ID:** 91843
- **MITRE Technique:** T1059.001 – PowerShell
- **Description:** PowerShell command execution detected

## PowerShell Detection Dashboard

The Wazuh dashboard displays PowerShell execution events, allowing analysts to investigate suspicious command execution and identify potential attacker activity.

![PowerShell Detection](../Screenshots/powershell-detection.png)
