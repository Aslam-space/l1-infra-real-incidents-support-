# Ticket ID: TICKET-016

## Issue Title
Server unable to resolve domain names

## Description
Applications failed to connect using domain names.

## User Reported Problem
Internet works but websites not loading by name.

## Initial Checks (L1)
- Tested ping with IP vs domain
- Checked /etc/resolv.conf

## Troubleshooting Performed
- Verified DNS server entries
- Tested name resolution using nslookup
- Updated DNS configuration

## Root Cause
Incorrect DNS server configuration.

## Resolution
Correct DNS entries added and tested.

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA

## Learning
DNS issues can appear as application failures.
