# Ticket ID: TICKET-002

## Issue Title
Disk usage alert – root partition at 95%

## User Reported Problem
Server alert: Disk nearly full, system slowing down.

## Initial Checks (L1)
- Ran `df -h` to check disk usage
- Identified affected partition
- Ran `du -sh /var/*` to find large directories

## Troubleshooting Performed
- Found log files consuming most space
- Cleared old log files safely
- Verified free space after cleanup
- Checked disk monitoring alert setup

## Root Cause
Logs were not rotated, filled the disk.

## Resolution
Old logs removed, disk usage reduced to normal levels.

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA time; no escalation required.

## Learning
Regular disk monitoring and log cleanup are critical L1 tasks.
