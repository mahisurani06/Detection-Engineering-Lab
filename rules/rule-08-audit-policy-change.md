# Detection Rule 08 – Audit Policy Change Monitoring

## Event ID

4719

## Objective

Detect changes to Windows audit policies.

## Why It Matters

Attackers may modify audit policies to disable logging and evade detection.

## Detection Logic

Alert whenever Event ID 4719 is generated.

## Severity

High

## MITRE ATT&CK

TA0005 – Defense Evasion

T1562.002 – Disable Security Tools

## Investigation Steps

1. Identify who changed the audit policy.
2. Determine what setting was modified.
3. Verify authorization for the change.
4. Review nearby security events.
5. Investigate possible malicious activity.

## Lab Result

No Event ID 4719 events found.

## Analyst Conclusion

No audit policy modifications detected.

Risk Level: Low