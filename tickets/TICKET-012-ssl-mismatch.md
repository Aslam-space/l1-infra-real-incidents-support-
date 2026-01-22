# Ticket ID: TICKET-012

## Issue Title
SSL certificate mismatch warning

## Description
Users reported security warning due to domain mismatch.

## User Reported Problem
Browser warning shows certificate issued for a different domain.

## Initial Checks (L1)
- Verified accessed domain name
- Checked SSL certificate CN/SAN fields
- Tested with alternate browsers

## Troubleshooting Performed
- Compared domain with certificate details
- Verified web server configuration
- Checked virtual host settings

## Root Cause
Incorrect SSL certificate applied to the domain.

## Resolution
- Installed correct SSL certificate
- Reloaded web server configuration
- Verified secure access

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA

## Learning
Always validate certificate-domain matching.
