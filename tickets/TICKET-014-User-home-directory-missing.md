# Ticket ID: TICKET-014

## Issue Title
User login fails due to missing home directory

## Description
User unable to log in to Linux system.

## User Reported Problem
Login fails immediately after entering credentials.

## Initial Checks (L1)
- Verified user exists
- Checked home directory path
- Checked permissions

## Troubleshooting Performed
- Verified user entry in /etc/passwd
- Identified missing home directory
- Recreated home directory
- Set correct ownership and permissions

## Root Cause
Home directory was accidentally deleted.

## Resolution
Home directory recreated and permissions restored.

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA

## Learning
Home directory permissions are critical for login.
