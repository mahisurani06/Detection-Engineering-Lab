# Detection Rule 05 – Privileged Group Membership Monitoring

## Event ID

4728

## Objective

Detect when a user is added to a privileged security group.

## Why It Matters

Attackers often add compromised accounts to privileged groups to gain administrative access and maintain persistence.

## Detection Logic

Alert whenever Event ID 4728 is generated.

## Severity

High

## MITRE ATT&CK

TA0004 – Privilege Escalation

T1098 – Account Manipulation

## Investigation Steps

1. Identify the account added.
2. Identify who performed the action.
3. Verify change approval.
4. Review recent login activity.
5. Check for suspicious administrative actions.

## Lab Result

No Event ID 4728 events were found.

## Analyst Conclusion

No privileged group membership modifications detected.

Risk Level: Low