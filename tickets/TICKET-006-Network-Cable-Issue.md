# Ticket ID: TICKET-006

## Issue Title
User reports no internet connectivity

## User Reported Problem
PC shows “Network cable unplugged” or cannot access internet

## Initial Checks (L1)
- Checked Ethernet cable physically connected
- Verified link lights on NIC port
- Tested with alternate port/cable

## Troubleshooting Performed
- Reseated cable and tested NIC
- Checked IP configuration (ipconfig / Windows, ifconfig / Linux)
- Checked DHCP assignment

## Root Cause
Loose cable connection

## Resolution
- Reconnected cable
- Verified internet connectivity
- Tested other devices to confirm network working

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA

## Learning
Physical connectivity is most common cause; always check cable before software/network troubleshooting.
