# Ticket ID: TICKET-007

## Category
L1 Infrastructure Support / Linux Support

## Priority
P2 (High)

## Issue Summary
Linux server service is down – application not accessible.

## Environment
- Server Type: Linux VM
- OS: Ubuntu 20.04
- Service Affected: Nginx
- Access Method: SSH

## User Reported Symptoms
User reported that the application URL is not loading and shows “site can’t be reached”.

## L1 Initial Assessment
- Verified server reachability using ping
- Confirmed SSH access to server
- Checked if issue is application or network related

## Troubleshooting Actions Performed
1. Logged into server via SSH
2. Checked service status using `systemctl status nginx`
3. Identified service was stopped
4. Reviewed logs using `journalctl -u nginx`
5. Restarted service using `systemctl restart nginx`
6. Verified service is active and listening on port 80

## Root Cause Analysis
Nginx service had stopped due to a previous configuration reload failure.

## Resolution Steps
- Restarted Nginx service
- Verified service status as running
- Confirmed application accessible via browser

## Validation
- Application URL loading successfully
- User confirmed issue resolved

## Escalation
Not required – issue resolved at L1 level.

## SLA & Impact
- Priority: P2
- Resolution Time: Within SLA
- Business Impact: Application downtime for users

## Key Learning
Always check service status and logs first before assuming network or server failure.
