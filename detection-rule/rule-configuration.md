# Detection Rule Configuration

## Rule Name

Failed Login Brute Force Detection

## Rule Type

Threshold Rule

## Data Source

Elastic Security Data View

## KQL Query

```kql
event.code:"4625"
```

## Group By

host.name

## Threshold

2 failed login events

## Schedule

Runs every 5 minutes
Additional look-back time: 1 minute

## Severity

Medium

## Risk Score

50

## Description

This detection rule identifies repeated failed Windows logon attempts originating from the same host.
The rule helps detect possible brute-force attacks or unauthorized authentication attempts.
