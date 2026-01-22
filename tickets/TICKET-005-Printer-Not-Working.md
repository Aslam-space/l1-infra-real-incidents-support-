# Ticket ID: TICKET-005

## Issue Title
User cannot print to network printer

## User Reported Problem
Printer shows offline / prints fail

## Initial Checks (L1)
- Verified printer is powered on
- Checked network connectivity (ping printer IP)
- Checked printer queue

## Troubleshooting Performed
- Restarted printer spooler service
- Reinstalled printer driver if needed
- Verified printer IP settings

## Root Cause
Printer spooler service had stopped

## Resolution
- Restarted service
- Verified print job success

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA

## Learning
Printer spooler failures are common; quick service restart fixes most issues.
