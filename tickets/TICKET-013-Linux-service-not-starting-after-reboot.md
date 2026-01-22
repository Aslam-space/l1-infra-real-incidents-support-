# Ticket ID: TICKET-013

## Issue Title
Linux service failed to start after server reboot

## Description
After scheduled reboot, application service did not start automatically.

## User Reported Problem
Application was unavailable after reboot.

## Initial Checks (L1)
- Verified server uptime
- Checked service status using systemctl
- Confirmed issue started after reboot

## Troubleshooting Performed
- Checked service status: `systemctl status <service>`
- Reviewed logs: `journalctl -u <service>`
- Verified service configuration file
- Checked if service was enabled at boot

## Root Cause
Service was disabled and had configuration warning.

## Resolution
- Fixed configuration issue
- Enabled service at boot
- Restarted service successfully

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA

## Learning
Always verify services are enabled to start on boot.
