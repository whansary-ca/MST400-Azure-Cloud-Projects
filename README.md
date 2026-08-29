# MST400 Azure Cloud Projects

Hands-on Microsoft Azure projects focused on cloud networking, secure remote access, disaster recovery, infrastructure monitoring, and operational troubleshooting.

These projects were completed through MST400 coursework at Seneca Polytechnic and are organized here as a cloud portfolio rather than as a single assignment.

## Projects

### 1. Azure Traffic Manager & Point-to-Site VPN

**Folder:** [`azure-traffic-manager-p2s-vpn`](./azure-traffic-manager-p2s-vpn)

Implemented multi-region Azure traffic routing and secure Point-to-Site remote connectivity.

**Highlights**
- Azure Traffic Manager and regional endpoints
- Azure VPN Gateway and Point-to-Site VPN
- Certificate-based authentication
- Azure VNets, subnets, NSGs, and virtual machines
- Private-IP SSH access to Ubuntu
- Routing, certificate, tunnel, and connectivity troubleshooting

### 2. Azure Backup & Site Recovery

**Folder:** [`azure-backup-site-recovery`](./azure-backup-site-recovery)

Implemented an end-to-end VM protection and disaster-recovery workflow.

**Highlights**
- ARM-template infrastructure deployment
- Recovery Services Vault and VM backup policy
- On-demand backup validation and restore points
- Diagnostic settings and backup-job monitoring
- Azure Site Recovery replication from East US to West US
- Verified Healthy/Protected replication state and approximately 1-minute RPO
- Troubleshot `UserErrorBackupOperationInProgress`

### 3. Azure Monitor & Log Analytics

**Folder:** [`azure-monitor-log-analytics`](./azure-monitor-log-analytics)

Built an Azure monitoring and observability workflow using alerts and KQL-based log analysis.

**Highlights**
- Azure Monitor alerts and action groups
- Alert processing rules
- Log Analytics workspace
- Kusto Query Language (KQL)
- Heartbeat and InsightsMetrics queries
- Performance visualization and cloud troubleshooting

## Core Technologies

`Microsoft Azure` · `Azure Traffic Manager` · `VPN Gateway` · `VNet` · `NSG` · `Azure VMs` · `Azure Backup` · `Recovery Services Vault` · `Azure Site Recovery` · `ARM Templates` · `Azure Monitor` · `Log Analytics` · `KQL` · `Ubuntu` · `SSH` · `X.509 Certificates`

## Skills Demonstrated

- Azure infrastructure administration
- Cloud networking and secure remote access
- Multi-region routing and resiliency
- Backup, recovery, replication, and business continuity
- Infrastructure-as-code concepts
- Monitoring, logging, alerting, and KQL
- Windows/Linux VM administration
- Cloud and network troubleshooting
- Technical documentation and validation

## Repository Structure

```text
MST400-Azure-Cloud-Projects/
├── azure-traffic-manager-p2s-vpn/
├── azure-backup-site-recovery/
└── azure-monitor-log-analytics/
```

Each project folder contains its own README and the original supporting files that are appropriate for GitHub.