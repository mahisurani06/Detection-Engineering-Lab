# Detection Rule 04 – User Account Creation Detection

## Event ID

4720

## Objective

Detect creation of new local or domain user accounts.

## Why It Matters

Attackers frequently create new accounts after gaining access to maintain persistence.

## Detection Logic

Alert when Event ID 4720 occurs.

## Severity

High

## MITRE ATT&CK

TA0003 – Persistence

T1136 – Create Account

## Investigation Steps

1. Identify newly created account.
2. Determine who created the account.
3. Verify whether account creation was authorized.
4. Check if account was added to privileged groups.
5. Review related account management events.

## Lab Result

No Event ID 4720 events were found on the system.

## Analyst Conclusion

No evidence of unauthorized account creation.

Risk Level: Low
