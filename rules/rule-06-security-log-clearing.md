# Detection Rule 06 – Security Log Clearing

## Event ID

1102

## Objective

Detect attempts to clear Windows Security logs.

## Why It Matters

Attackers often clear logs after gaining access to hide their actions and remove forensic evidence.

## Detection Logic

Alert whenever Event ID 1102 is generated.

## Severity

Critical

## MITRE ATT&CK

TA0005 – Defense Evasion

T1070.001 – Clear Windows Event Logs

## Investigation Steps

1. Identify the user who cleared the logs.
2. Determine when the logs were cleared.
3. Review activity before the event.
4. Investigate privilege escalation events.
5. Check for persistence mechanisms.

## Lab Result

No Event ID 1102 events found.

## Analyst Conclusion

No evidence of security log tampering.

Risk Level: Low