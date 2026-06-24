## Detection Engineering Lab – Windows Event Monitoring and Sigma Rule Development

## Project Overview

This project demonstrates practical Detection Engineering and SOC Analyst skills through the analysis of Windows Security and System Event Logs.

The objective was to identify critical security events, develop detection rules, create Sigma signatures, map detections to the MITRE ATT&CK framework, and document investigation procedures similar to real-world Security Operations Center (SOC) workflows.

---

## Technologies Used

* Windows 11
* Windows Event Viewer
* Windows Security Logs
* Sigma Rules
* MITRE ATT&CK Framework
* Git & GitHub

---

## Detection Rules Developed

| Rule    | Event ID | Detection                              |
| ------- | -------- | -------------------------------------- |
| Rule 01 | 4688     | Process Creation Monitoring            |
| Rule 02 | 4625     | Failed Login Detection                 |
| Rule 03 | 4624     | Successful Login Monitoring            |
| Rule 04 | 4720     | User Account Creation Detection        |
| Rule 05 | 4728     | Privileged Group Membership Monitoring |
| Rule 06 | 1102     | Security Log Clearing Detection        |
| Rule 07 | 4698     | Scheduled Task Creation Detection      |
| Rule 08 | 4719     | Audit Policy Change Detection          |
| Rule 09 | 7045     | Service Installation Detection         |

---

## Sigma Rules Created

### Failed Login Detection

* Event ID: 4625
* MITRE ATT&CK: T1110 (Brute Force)

### Process Creation Detection

* Event ID: 4688
* MITRE ATT&CK: T1059 (Command and Scripting Interpreter)

### Service Installation Detection

* Event ID: 7045
* MITRE ATT&CK: T1543 (Create or Modify System Process)

---

## MITRE ATT&CK Mapping

| Event ID | Technique ID | Technique                         |
| -------- | ------------ | --------------------------------- |
| 4625     | T1110        | Brute Force                       |
| 4624     | T1078        | Valid Accounts                    |
| 4688     | T1059        | Command and Scripting Interpreter |
| 4720     | T1136        | Create Account                    |
| 4728     | T1098        | Account Manipulation              |
| 1102     | T1070        | Indicator Removal on Host         |
| 4698     | T1053        | Scheduled Task                    |
| 4719     | T1562        | Impair Defenses                   |
| 7045     | T1543        | Create or Modify System Process   |

---

## Validation Activities

The following activities were performed to generate and validate Windows security events:

* Created process execution events using Notepad, Calculator, and Paint
* Generated successful login events
* Generated failed login events
* Investigated service installation events
* Reviewed Windows Security and System logs
* Validated Event IDs through Event Viewer

Screenshots are available in the `screenshots/` directory.

---

## Key Skills Demonstrated

* Detection Engineering
* Security Monitoring
* Windows Event Log Analysis
* Threat Detection
* Incident Investigation
* Sigma Rule Development
* MITRE ATT&CK Mapping
* SOC Operations
* Security Documentation
* GitHub Project Management

---

## Repository Structure

```text
Detection-Engineering-Lab/
│
├── docs/
├── rules/
├── sigma-rules/
├── screenshots/
└── README.md
```

---

## Author

**Mahi Surani**

Cybersecurity Student | SOC Analyst Aspirant | Detection Engineering Enthusiast
