# Ticket ID: TICKET-008

## Issue Title
High CPU and memory utilization causing system slowness

## Description
Linux server performance issue where CPU and memory usage were consistently high, affecting application response time.

## User Reported Problem
User reported system lag and slow application performance.

## Initial Checks (L1)
- Checked system load using `uptime`
- Verified CPU and memory usage using `top` and `free -m`
- Identified top resource-consuming processes

## Troubleshooting Performed
- Used `top` and `htop` to identify high CPU process
- Checked process details using `ps aux --sort=-%cpu`
- Verified if issue was recurring or one-time spike
- Checked logs related to the service causing high usage
- Restarted the affected service after confirmation

## Root Cause
A misbehaving application process was consuming excessive CPU and memory.

## Resolution
- Restarted the problematic service
- CPU and memory usage returned to normal levels
- Monitored system performance post-fix

## Status
Resolved at L1 level

## SLA Impact
Resolved within SLA; no escalation required

## Learning
Always identify the process causing high usage before restarting or escalating.
