# Process Creation Investigation

## Alert

Event ID: 4688

## Description

A new process was created on the endpoint.

## Observed Process

Notepad.exe

## Investigation Steps

1. Verified parent process.
2. Confirmed execution by authorized user.
3. Checked command line arguments.
4. Reviewed surrounding security events.

## MITRE ATT&CK

T1059 – Command and Scripting Interpreter

## Verdict

Benign activity.