\# Brute Force Attack Detection



\## Overview



This document explains how Wazuh detected a brute force attack against the monitored system by analyzing authentication logs generated during multiple failed SSH login attempts.



\## Lab Environment



\- Wazuh Manager: Ubuntu Server 22.04

\- Wazuh Version: 4.12.0

\- Endpoint: Ubuntu Server (OpenSSH)

\- Virtualization Platform: VirtualBox



\## Objectives



\- Simulate a brute force attack

\- Detect repeated failed SSH login attempts

\- Generate security alerts in Wazuh

\- Investigate attack activity using the Wazuh Dashboard



\## Attack Simulation



A brute force attack was simulated by repeatedly attempting to log in through SSH using invalid credentials.



This generated multiple failed authentication events that were collected and analyzed by Wazuh.



\## Detection Results



Wazuh successfully detected:



\- Multiple failed SSH login attempts

\- Authentication failures

\- Brute force attack indicators

\- High-severity security alerts



The alerts appeared in the Wazuh Dashboard immediately after the attack simulation.



\## MITRE ATT\&CK Mapping



\- Tactic: Credential Access

\- Technique: T1110 – Brute Force



\## Skills Demonstrated



\- Security Monitoring

\- Log Analysis

\- Authentication Monitoring

\- Brute Force Detection

\- Threat Investigation

\- MITRE ATT\&CK Mapping

\- Wazuh SIEM



\## Result



The simulated brute force attack was successfully detected by Wazuh. Authentication logs were analyzed in real time, alerts were generated automatically, and the attack was mapped to the MITRE ATT\&CK framework, demonstrating effective threat detection capabilities.

