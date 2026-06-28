# Detection Rule Configuration

## Rule Name

Failed Login Brute Force Detection

## Rule Type

Threshold Rule

## Data Source

Security Solution Default (Elastic Security Data View)

## KQL Query

```kql
event.code:"4625"
```

## Group By

host.name

## Threshold

Generate an alert when 2 or more failed login events are detected from the same host.

## Schedule

Runs every 5 minutes
Additional look-back time: 1 minute

## Severity

Medium

## Risk Score

50

## Description

This detection rule identifies repeated failed Windows logon attempts originating from the same host.
The rule helps detect possible brute-force attacks or unauthorized authentication attempts by generating an alert when the configured threshold is reached.
