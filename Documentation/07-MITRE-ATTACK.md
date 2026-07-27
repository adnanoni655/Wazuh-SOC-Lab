# MITRE ATT&CK Investigation

## Overview

This document demonstrates how Wazuh maps security events to the MITRE ATT&CK framework, helping analysts understand attacker tactics and techniques. During this lab, PowerShell execution and authentication events were automatically associated with relevant MITRE ATT&CK techniques, providing valuable context for threat investigation.

## Lab Environment

- **Manager:** Wazuh 4.12.0
- **Operating System:** Ubuntu Server 22.04 LTS
- **Endpoint:** Windows 10 Home
- **Virtualization Platform:** Oracle VirtualBox

## Objectives

- Analyze security alerts using the MITRE ATT&CK framework
- Identify attacker tactics and techniques
- Correlate alerts with endpoint activity
- Improve threat investigation and incident response

## Steps Performed

1. Generated security events on the Windows endpoint.
2. Collected logs using the Wazuh Agent.
3. Reviewed alerts in the Wazuh Dashboard.
4. Examined the MITRE ATT&CK mappings associated with each alert.
5. Investigated the related tactics and techniques.

## Investigation Results

Wazuh automatically enriched security alerts with MITRE ATT&CK information, making it easier to understand the nature of detected activity.

Examples observed during the lab include:

| Technique ID | Technique | Tactic |
|--------------|-----------|--------|
| T1059.001 | PowerShell | Execution |
| T1110 | Brute Force | Credential Access |

By mapping alerts to the MITRE ATT&CK framework, analysts can better prioritize investigations, understand attacker behavior, and respond more effectively to potential threats.

## MITRE ATT&CK Dashboard

The Wazuh dashboard provides built-in MITRE ATT&CK mappings, allowing analysts to quickly correlate alerts with known adversary techniques.

![MITRE ATT&CK Dashboard](../Screenshots/mitre-attack-dashboard.png)
