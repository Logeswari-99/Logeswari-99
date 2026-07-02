# VMware & Windows Server Administration

Hi, I'm Logeswari — a VMware and Windows Server Administrator with hands-on experience managing vSphere environments, Active Directory, and day-to-day infrastructure operations.
This repository contains a collection of PowerShell and PowerCLI scripts I've written to automate common administrative tasks: health checks, reporting, cleanup, provisioning, and alerting. I built these to demonstrate the kind of automation work I do (or want to do) in a production environment.

## 🧰 Tech / Skills
- VMware vSphere / ESXi / vCenter administration
- Windows Server (2016/2019/2022) administration
- Active Directory, Group Policy
- PowerShell & PowerCLI scripting
- Automation, monitoring, and reporting

## 📂 Scripts in this portfolio

| # | Script | What it does | Area |
|---|--------|---------------|------|
| 1 | [Get-VMHealthReport](./01-vmware-vm-health-report) | Reports on VM CPU/RAM/disk usage and flags issues | VMware |
| 2 | [Remove-OldSnapshots](./02-snapshot-cleanup) | Finds and (optionally) removes old VM snapshots | VMware |
| 3 | [Send-DatastoreAlert](./03-datastore-usage-alert) | Alerts when datastore free space drops below threshold | VMware |
| 4 | [New-VMFromTemplate](./04-vm-provisioning) | Automates VM provisioning from a template | VMware |
| 5 | [Get-ADUserReport](./05-ad-bulk-user-report) | Reports on stale, disabled, and expiring AD accounts | Active Directory |
| 6 | [Send-PasswordExpiryNotice](./06-ad-password-expiry-notification) | Emails users before their AD password expires | Active Directory |
| 7 | [Get-ServerHealthCheck](./07-windows-server-health-check) | Checks disk space, services, and event log errors on Windows Servers | Windows Server |
| 8 | [Backup-GPOs](./08-gpo-backup) | Backs up all Group Policy Objects on a schedule | Active Directory |

Each folder has its own README with usage instructions, parameters, and sample
output.

## ⚠️ A note on safety

All scripts default to **read-only / reporting mode**. Anything destructive
(like deleting snapshots) requires an explicit switch to actually make
changes, and supports `-WhatIf` where applicable. This mirrors how I approach
changes in production: report first, act deliberately.

## 📫 Contact

- LinkedIn: [https://www.linkedin.com/in/logeswari99/]
- Email: [logeswarinirmala@gmail.com]
