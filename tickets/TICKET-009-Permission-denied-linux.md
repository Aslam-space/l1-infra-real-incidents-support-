# Ticket ID: TICKET-009

## Issue Title
Permission denied error while accessing application files

## Description
User was unable to access or modify files required by an application due to permission issues on a Linux server.

## User Reported Problem
Application failed with “Permission denied” error when accessing files.

## Initial Checks (L1)
- Verified exact error message
- Checked file and directory permissions using `ls -l`
- Checked file ownership using `ls -l`
- Verified which user/service was accessing the file

## Troubleshooting Performed
- Identified incorrect ownership on application directory
- Verified required permissions for user/service
- Used `chmod` to adjust permissions
- Used `chown` to correct file ownership
- Ensured permissions followed least-privilege principle

## Root Cause
Incorrect file ownership and permissions caused application access failure.

## Resolution
- Corrected ownership using `chown`
- Updated permissions using `chmod`
- Verified application access and functionality

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA; no escalation required

## Learning
Always verify ownership before changing permissions. Avoid giving 777 permissions.
