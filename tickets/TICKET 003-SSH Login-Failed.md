# Ticket ID: TICKET-003

## Issue Title
User unable to SSH into Linux server

## User Reported Problem
User reports they cannot connect to server using SSH.

## Initial Checks (L1)
- Verified server is reachable (ping <server-ip>)
- Checked correct username and IP
- Checked if SSH service is running

## Troubleshooting Performed
- Ran `systemctl status sshd` to verify service
- Checked `/var/log/auth.log` for authentication errors
- Verified permissions on `~/.ssh` and `authorized_keys`
- Confirmed firewall is not blocking port 22

## Root Cause
SSH service was stopped / incorrect file permissions.

## Resolution
- Restarted SSH service
- Corrected file permissions
- Verified successful login

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA time; no escalation required.

## Learning
Check network reachability, service status, permissions, and logs before escalating.
