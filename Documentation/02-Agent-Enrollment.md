\# Windows Agent Enrollment



\## Overview



This document explains how the Windows 10 endpoint was enrolled into the Wazuh Security Information and Event Management (SIEM) platform for centralized monitoring.



\## Lab Environment



\- Wazuh Manager: Ubuntu Server 22.04

\- Wazuh Version: 4.12.0

\- Endpoint: Windows 10 Home

\- Connection: VirtualBox Internal Network



\## Objectives



\- Install the Wazuh Agent

\- Connect the endpoint to the Wazuh Manager

\- Verify successful communication

\- Begin centralized log collection



\## Installation Process



1\. Downloaded the Wazuh Windows Agent.

2\. Installed the agent on the Windows endpoint.

3\. Configured the manager IP address.

4\. Started the Wazuh Agent service.

5\. Verified that the endpoint appeared in the Wazuh Dashboard.



\## Result



The Windows endpoint successfully connected to the Wazuh Manager. Once enrolled, the system began sending security events, allowing centralized monitoring and enabling later exercises such as File Integrity Monitoring, Windows Defender monitoring, PowerShell monitoring, brute-force detection, vulnerability detection, and MITRE ATT\&CK mapping.



\## Skills Demonstrated



\- SIEM Deployment

\- Endpoint Management

\- Windows Administration

\- Log Collection

\- Security Monitoring

