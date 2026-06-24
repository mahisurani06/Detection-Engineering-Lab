# Detection Rule 07 – Scheduled Task Creation

## Event ID

4698

## Objective

Detect creation of new scheduled tasks.

## Why It Matters

Scheduled tasks are commonly abused by attackers to maintain persistence and execute malicious payloads automatically.

## Detection Logic

Alert whenever Event ID 4698 is generated.

## Severity

High

## MITRE ATT&CK

TA0003 – Persistence

T1053.005 – Scheduled Task

## Investigation Steps

1. Identify the task name.
2. Review task action and executable path.
3. Verify creator account.
4. Check related process creation events.
5. Determine whether the task is legitimate.

## Lab Result

No Event ID 4698 events found.

## Analyst Conclusion

No suspicious scheduled task creation detected.

Risk Level: Low