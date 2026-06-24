# Detection Rule 02 – Failed Login Detection

## Objective

Detect failed login attempts that may indicate brute-force attacks or unauthorized access attempts.

## Event ID

4625 – Failed Logon

## Detection Logic

Trigger alert when:

* Event ID = 4625
* Same account generates 5 or more failures
* Within 5 minutes

## Severity

Medium

## MITRE ATT&CK

T1110 – Brute Force

## Observed Event

Account Name:
VICTUS

Failure Reason:
Unknown user name or bad password

Status:
0xC000006D

SubStatus:
0xC000006A

Source IP:
127.0.0.1

Logon Type:
2 (Interactive)

## Investigation Steps

1. Identify affected account.
2. Count failed logins.
3. Check source IP address.
4. Look for successful login events (4624).
5. Determine whether brute force activity exists.

## Analyst Conclusion

Single failed login detected.

No evidence of brute-force activity.

Risk Level: Low
