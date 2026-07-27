# Windows Agent Enrollment

## Overview

This document explains how I enrolled a Windows 10 Home endpoint into my Wazuh Security Operations Center (SOC) lab. After installing the Wazuh agent, the endpoint began sending security events to the Wazuh Manager for centralized monitoring and analysis.

## Lab Environment

- **Manager:** Wazuh 4.12.0
- **Operating System:** Ubuntu Server 22.04 LTS
- **Endpoint:** Windows 10 Home
- **Virtualization Platform:** VirtualBox

## Objectives

- Install the Wazuh Agent on Windows
- Connect the endpoint to the Wazuh Manager
- Verify successful communication
- Confirm the endpoint appears in the Wazuh Dashboard

## Steps Performed

1. Downloaded the Windows Wazuh Agent.
2. Installed the agent on the Windows 10 endpoint.
3. Configured the agent to communicate with the Wazuh Manager.
4. Started the Wazuh Agent service.
5. Verified successful registration in the Wazuh Dashboard.

## Result

The Windows endpoint successfully connected to the Wazuh Manager and began sending security events. The endpoint appeared as an active agent in the dashboard, enabling centralized monitoring and future security detection capabilities.

## Registered Agent

The dashboard confirms that the Windows endpoint has successfully enrolled and is actively communicating with the Wazuh Manager.

![Registered Agent](../Screenshots/Agents.png)
