# Brute Force Detection

## Overview

This document explains how I simulated and detected a brute force attack in my Wazuh SOC lab. Since Windows 10 Home does not include an RDP server, I configured an OpenSSH server on the Windows endpoint and generated multiple failed login attempts to trigger security alerts.

## Lab Environment

- **Manager:** Wazuh 4.12.0
- **Operating System:** Ubuntu Server 22.04 LTS
- **Endpoint:** Windows 10 Home
- **Virtualization Platform:** VirtualBox

## Objectives

- Enable SSH access on the Windows endpoint
- Generate failed authentication attempts
- Detect brute force activity
- Verify alerts in the Wazuh Dashboard

## Steps Performed

1. Enabled the OpenSSH Server feature on Windows 10 Home.
2. Connected from another system using SSH.
3. Entered incorrect passwords multiple times to simulate a brute force attack.
4. Allowed the Wazuh Agent to collect Windows security events.
5. Verified authentication failure alerts in the Wazuh Dashboard.

## Result

Wazuh successfully detected multiple failed authentication attempts and generated security alerts. These events demonstrate the platform's ability to identify potential brute force attacks and provide analysts with early warning of unauthorized access attempts.

## Authentication Failure Detection

The Wazuh dashboard displays authentication failure events generated during the simulated brute force attack, enabling analysts to investigate suspicious login activity.

![Authentication Failure](../Screenshots/authentication-failure.png)
