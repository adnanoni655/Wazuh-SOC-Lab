# Wazuh Installation

## Overview

This document explains how I installed and configured the Wazuh Security Information and Event Management (SIEM) platform as the foundation of my home SOC lab.

## Lab Environment

- **Wazuh Version:** 4.12.0
- **Operating System:** Ubuntu Server 22.04 LTS
- **Virtualization Platform:** Oracle VirtualBox
- **Endpoint:** Windows 10 Home

## Objectives

- Install and configure the Wazuh Manager
- Access the Wazuh Dashboard
- Prepare the environment for endpoint monitoring
- Build a foundation for future security monitoring and incident response

## Result

The Wazuh Manager was successfully installed and configured. The Wazuh dashboard became accessible, allowing additional security capabilities such as File Integrity Monitoring (FIM), Vulnerability Detection, Windows Defender monitoring, Configuration Assessment, and MITRE ATT&CK mapping to be implemented.

## Dashboard Overview

The Wazuh dashboard provides centralized visibility into the security posture of monitored endpoints. From a single interface, analysts can review agent status, monitor security events, investigate alerts, assess vulnerabilities, perform configuration assessments, and analyze MITRE ATT&CK techniques.

![Wazuh Dashboard](../Screenshots/Wazuh-Overview.png)
