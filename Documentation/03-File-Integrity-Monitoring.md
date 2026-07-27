\# File Integrity Monitoring (FIM)



\## Overview



This document explains how File Integrity Monitoring (FIM) was configured in Wazuh to detect unauthorized changes made to files on the monitored Windows endpoint.



\## Lab Environment



\- Wazuh Manager: Ubuntu Server 22.04

\- Wazuh Version: 4.12.0

\- Endpoint: Windows 10 Home

\- Virtualization Platform: VirtualBox



\## Objectives



\- Enable File Integrity Monitoring

\- Monitor important files on the Windows endpoint

\- Detect file creation, modification, and deletion

\- Generate security alerts in the Wazuh Dashboard



\## Configuration



The Wazuh agent was configured to monitor selected directories on the Windows endpoint.



The Wazuh Manager continuously compared file metadata and generated alerts whenever changes were detected.



\## Testing



The following actions were performed:



1\. Created a test file.

2\. Modified the contents of the file.

3\. Deleted the file.

4\. Verified that Wazuh detected each action.



\## Detection Results



Wazuh successfully detected:



\- File Creation

\- File Modification

\- File Deletion



The alerts appeared in the Wazuh Dashboard, confirming that File Integrity Monitoring was functioning correctly.



\## Skills Demonstrated



\- Endpoint Monitoring

\- File Integrity Monitoring (FIM)

\- Security Event Analysis

\- Log Investigation

\- Threat Detection

\- Wazuh SIEM



\## Result



File Integrity Monitoring was successfully configured and validated. Wazuh generated alerts whenever monitored files changed, demonstrating an important capability for detecting unauthorized modifications on enterprise systems.

