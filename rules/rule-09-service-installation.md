# Detection Rule 09 – Service Installation Monitoring

## Event ID

7045

## Objective

Detect installation of new Windows services.

## Why It Matters

Attackers frequently install services to maintain persistence and execute malware automatically.

## Detection Logic

Alert whenever Event ID 7045 is generated.

## Severity

High

## MITRE ATT&CK

TA0003 – Persistence

T1543.003 – Create or Modify System Process: Windows Service

## Investigation Steps

1. Identify service name.
2. Review executable path.
3. Verify digital signature.
4. Determine installer source.
5. Check related process creation events.

## Lab Result

26 service installation events identified.

Example:

Service Name:
VirtualBox system service

Executable:
C:\Program Files\Oracle\VirtualBox\VBoxSDS.exe

Assessment:
Legitimate VirtualBox installation.

## Analyst Conclusion

Service installation activity observed.

Reviewed event was determined to be legitimate software installation.

Risk Level: Low