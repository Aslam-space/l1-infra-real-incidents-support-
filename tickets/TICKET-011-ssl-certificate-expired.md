# Ticket ID: TICKET-011

## Issue Title
Website shows SSL certificate expired error

## Description
Users reported browser security warning when accessing company website.

## User Reported Problem
Website not opening; browser displays “Your connection is not private”.

## Initial Checks (L1)
- Verified website URL
- Checked certificate expiry date via browser
- Confirmed issue across multiple devices

## Troubleshooting Performed
- Checked SSL certificate validity
- Verified domain and certificate chain
- Confirmed hosting server accessibility

## Root Cause
SSL certificate expired and was not renewed automatically.

## Resolution
- Renewed SSL certificate
- Restarted web service
- Verified HTTPS access restored

## Status
Resolved at L1 level

## SLA Impact
Service disruption resolved within SLA

## Learning
SSL expiry monitoring is critical for production systems.
