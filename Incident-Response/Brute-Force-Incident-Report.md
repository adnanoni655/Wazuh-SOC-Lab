\# Incident Response Report: Brute Force Attack Detection



\## Executive Summary



This report documents the investigation of a simulated brute force attack detected by Wazuh in a home Security Operations Center (SOC) lab. Multiple failed SSH authentication attempts triggered security alerts, allowing the incident to be identified, analyzed, and documented.



\---



\## Incident Information



| Item | Value |

|------|-------|

| Incident Type | Brute Force Attack |

| Severity | Medium |

| Detection Tool | Wazuh SIEM |

| Endpoint | Windows 10 Home |

| Detection Method | Multiple Failed SSH Authentication Attempts |

| MITRE ATT\&CK | T1110 – Brute Force |



\---



\## Detection



Wazuh generated authentication failure alerts after repeated unsuccessful SSH login attempts against the Windows endpoint.



The alerts indicated:



\- Multiple failed login attempts

\- Repeated authentication failures

\- Potential password guessing activity



\---



\## Investigation



The investigation included the following steps:



1\. Reviewed authentication failure alerts in the Wazuh Dashboard.

2\. Examined timestamps to identify repeated login attempts.

3\. Confirmed the source of the SSH connections.

4\. Verified that no successful login occurred.

5\. Correlated the alerts with MITRE ATT\&CK Technique T1110 (Brute Force).



\---



\## Impact Assessment



No unauthorized access was achieved during the simulation.



The activity was generated intentionally for testing purposes and successfully demonstrated Wazuh's ability to detect repeated authentication failures.



\---



\## MITRE ATT\&CK Mapping



| Technique ID | Technique | Tactic |

|--------------|-----------|--------|

| T1110 | Brute Force | Credential Access |



\---



\## Response Actions



The following actions would be recommended in a production environment:



\- Block the attacking IP address.

\- Enforce strong password policies.

\- Enable Multi-Factor Authentication (MFA).

\- Implement account lockout policies.

\- Continue monitoring authentication events for repeated activity.



\---



\## Lessons Learned



This exercise demonstrated the effectiveness of Wazuh in detecting brute force attacks through authentication monitoring. Mapping alerts to the MITRE ATT\&CK framework provided additional context, enabling faster analysis and response.



\---



\## Conclusion



The simulated attack successfully validated Wazuh's ability to detect and alert on brute force activity. This lab highlights the importance of centralized log collection, continuous monitoring, and structured incident response procedures in modern Security Operations Centers.

