# Ticket ID: TICKET-004

## Issue Title
User unable to login to Windows PC

## User Reported Problem
User reports that login fails with “Incorrect password” even though credentials are correct.

## Initial Checks (L1)
- Confirmed username entered correctly
- Checked Num Lock / Caps Lock status
- Checked domain connectivity (if on corporate network)

## Troubleshooting Performed
- Verified network connectivity to domain controller
- Reset user password if allowed at L1
- Checked local profile corruption

## Root Cause
User account was temporarily locked due to multiple failed attempts

## Resolution
- Unlocked the account
- Instructed user on correct password usage
- Verified successful login

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA; no escalation required

## Learning
Check locks, network connectivity, and user environment before escalating.
