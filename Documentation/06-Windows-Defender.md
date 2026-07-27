# Windows Defender Monitoring

## Overview

This document explains how I integrated Microsoft Defender Antivirus with Wazuh to monitor endpoint protection events. Wazuh collected Windows Defender Operational logs and generated alerts whenever suspicious or potentially unwanted software was detected.

## Lab Environment

- **Manager:** Wazuh 4.12.0
- **Operating System:** Ubuntu Server 22.04 LTS
- **Endpoint:** Windows 10 Home
- **Virtualization Platform:** Oracle VirtualBox

## Objectives

- Monitor Microsoft Defender events
- Collect Windows Defender Operational logs
- Detect malware and potentially unwanted software
- Verify alerts in the Wazuh Dashboard

## Steps Performed

1. Verified that Microsoft Defender Real-Time Protection was enabled.
2. Configured the Wazuh Agent to monitor the Windows Defender Operational event log.
3. Generated a Microsoft Defender detection event for testing.
4. Allowed the Wazuh Agent to forward the event to the Wazuh Manager.
5. Verified that the alert appeared in the Wazuh Dashboard.

## Detection Results

Wazuh successfully detected Microsoft Defender events and generated security alerts.

Example detection:

- **Rule ID:** 62123
- **Rule Level:** 12
- **Description:** Windows Defender detected potentially unwanted software.

These alerts provide centralized visibility into endpoint protection events and allow analysts to investigate security incidents quickly.

## Windows Defender Detection

The Wazuh dashboard displays Microsoft Defender alerts, helping security analysts identify malware-related activity and endpoint protection events.

![Windows Defender Detection](../Screenshots/windows-defender-detection.png)
