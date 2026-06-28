# KQL Query

This project uses the following Kibana Query Language (KQL) query to identify failed Windows logon attempts.
```kql
event.code:"4625"
```

# Description

Windows Security Event ID **4625** indicates a failed logon attempt.
This query searches for all failed authentication events collected by Elastic Agent and visualized inside Elastic SIEM.
