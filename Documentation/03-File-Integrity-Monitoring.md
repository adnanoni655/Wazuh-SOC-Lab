# File Integrity Monitoring

## Overview

This document explains how I configured File Integrity Monitoring (FIM) in Wazuh to detect changes to files on the monitored Windows endpoint. FIM is an important security capability that helps identify unauthorized file creation, modification, and deletion.

## Lab Environment

- **Manager:** Wazuh 4.12.0
- **Operating System:** Ubuntu Server 22.04 LTS
- **Endpoint:** Windows 10 Home
- **Virtualization Platform:** VirtualBox

## Objectives

- Configure File Integrity Monitoring
- Monitor critical files for changes
- Generate file modification events
- Verify alerts in the Wazuh Dashboard

## Steps Performed

1. Enabled File Integrity Monitoring on the Windows endpoint.
2. Selected files and directories to monitor.
3. Modified monitored files to generate security events.
4. Allowed the Wazuh Agent to send events to the Manager.
5. Verified the alerts in the Wazuh Dashboard.

## Result

Wazuh successfully detected file modifications on the monitored endpoint. Alerts were generated whenever monitored files changed, demonstrating that File Integrity Monitoring was functioning correctly.

## File Integrity Monitoring Dashboard

The Wazuh dashboard displays file modification events, allowing security analysts to quickly identify unauthorized or suspicious changes.

![File Integrity Monitoring](../Screenshots/file-integrity-monitoring.png)
