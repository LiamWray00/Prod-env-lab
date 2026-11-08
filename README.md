# Prod-env-lab

## What this is
A small lab environment on Proxmox with two network segments, a router/firewall, internal DNS, DHCP, NAT, a web service built by Ansible, monitoring with alerts, centralized logging, and automated backups.

## Goal (done when)
I can destroy the server and rebuild it with one command, restore from backup without looking anything up, explain any packet in my capture, and show how each outage affected my reliability target.

## Build
- Two network segments with a Linux router/firewall, DHCP, internal DNS, and NAT
- Web service on the servers segment, provisioned by an Ansible playbook from a blank VM
- Prometheus and Grafana with alerts on disk, memory, and service down
- Centralized logging
- Automated backups with a written restore procedure
- Reliability target and error budget for the web service

## Break (failure drills)
Wrong gateway, bad DNS record, firewall rule that silently drops a protocol, full disk, killed service, corrupted config. Each has a case file.

## Status


## What I would change
