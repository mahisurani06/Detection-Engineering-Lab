# Detection Rule 01 – Suspicious LSASS Process Creation

## Objective

Detect suspicious creation of LSASS process from unexpected parent processes.

## Event ID

4688 – Process Creation

## Legitimate Behavior

Parent Process:
C:\Windows\System32\wininit.exe

Child Process:
C:\Windows\System32\lsass.exe

## Suspicious Behavior

Parent Process NOT equal to:

C:\Windows\System32\wininit.exe

AND

Child Process:

C:\Windows\System32\lsass.exe

## Severity

High

## MITRE ATT&CK

TA0006 – Credential Access

## Investigation Steps

1. Identify parent process.
2. Review command line.
3. Check user account.
4. Investigate related events.
5. Search for malware indicators.

## Analyst Notes

Normal Event Observed:

Parent:
C:\Windows\System32\wininit.exe

Child:
C:\Windows\System32\lsass.exe

Result:
Legitimate Windows Activity
