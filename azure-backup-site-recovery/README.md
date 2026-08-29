# Azure Backup & Site Recovery

## Overview

This MST400 cloud lab implemented an end-to-end business-continuity and disaster-recovery workflow for an Azure virtual machine. A Windows Server VM and its network resources were provisioned using an ARM template, protected with Azure Backup, monitored through Recovery Services and diagnostic settings, and replicated from East US to West US using Azure Site Recovery.

## What I Implemented

- Provisioned a Windows Server VM, VNet, subnet, NIC, NSG, public IP, and managed disk using an ARM template.
- Created and configured an Azure Recovery Services vault.
- Configured a Standard daily VM backup policy.
- Ran and validated an on-demand VM backup.
- Verified backup-job subtasks including snapshot creation, data transfer to the vault, and validation.
- Configured diagnostic settings to archive Azure Backup and Site Recovery logs and metrics to a storage account.
- Created a second Recovery Services vault in West US.
- Enabled Azure Site Recovery replication from East US to West US.
- Verified replication health as Healthy, protection status as Protected, and an RPO of approximately 1 minute.

## Troubleshooting

During testing, a second backup request was submitted while the first backup operation was still running. Azure returned `UserErrorBackupOperationInProgress`. I reviewed the failed job details, identified the duplicate operation, allowed the original job to complete, and then verified that a usable restore point had been created.

Initial Site Recovery synchronization also required monitoring until the replicated VM changed from synchronization in progress to Protected.

## Technologies

- Microsoft Azure
- Azure Virtual Machines
- Azure Backup
- Recovery Services Vault
- Azure Site Recovery
- ARM Templates
- Azure Virtual Network
- Network Security Groups
- Azure Storage
- Azure Monitor
- Diagnostic Settings

## Skills Demonstrated

Cloud infrastructure provisioning, infrastructure as code concepts, VM backup and recovery, cross-region disaster recovery, monitoring, diagnostics, troubleshooting, Azure networking, resiliency, and business continuity.
