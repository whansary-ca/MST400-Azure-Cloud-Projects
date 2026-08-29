# Azure Monitor & Log Analytics

## Overview

This MST400 monitoring lab focused on observing Azure infrastructure health and performance using Azure Monitor, alerts, action groups, alert processing rules, Log Analytics, and Kusto Query Language (KQL).

## What I Implemented

- Provisioned Azure infrastructure for monitoring and alert testing.
- Created Azure Monitor alerts and configured action-group notifications.
- Triggered and validated alert behavior.
- Configured an alert processing rule.
- Used Azure Monitor Logs and a Log Analytics workspace to query VM telemetry.
- Queried the `Heartbeat` table to confirm monitored VM connectivity and activity.
- Used KQL aggregation such as `Heartbeat | summarize count() by Computer`.
- Queried performance data using `InsightsMetrics`, including utilization metrics.
- Rendered KQL query results as charts for operational visibility.

## Example KQL

```kusto
Heartbeat
| summarize count() by Computer
```

The monitoring results identified the lab VM (`whansary-vm0`) and confirmed heartbeat telemetry reaching Log Analytics.

## Technologies

- Microsoft Azure
- Azure Monitor
- Log Analytics Workspace
- Kusto Query Language (KQL)
- Azure Alerts
- Action Groups
- Alert Processing Rules
- Azure Virtual Machines
- InsightsMetrics
- Heartbeat telemetry

## Skills Demonstrated

Cloud monitoring, observability, alert configuration, log analysis, KQL querying, performance visualization, infrastructure troubleshooting, and operational monitoring.
