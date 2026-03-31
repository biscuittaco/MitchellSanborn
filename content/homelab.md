# Homelab

![Server Rack](/img/serverrack.jpeg)

The homelab is part testing ground, part personal infrastructure, and part 
proving ground for things I want to understand before rolling them out anywhere 
else. It's where I break things on purpose, learn how they go back together, 
and run services my family actually depends on.

## Hardware

The lab runs across three primary systems:

- **Custom-built PC** with a Ryzen 7 3700x and 32GB RAM, used for lightweight 
  workloads and Docker containers.
- **Dual-node Supermicro SYS-2028TP-DC1R**, each node running dual Xeon 
  E5-2643 v4 CPUs and 128GB RAM. This is where most of the heavy lifting happens.
- **TrueNAS server** for storage, served over NFS and used as a Proxmox Backup 
  target among other things.

## Networking

Network management runs through a **UniFi Dream Machine Pro** with full VLAN 
segmentation throughout. A few specifics:

- **Site Magic** maintains a persistent VPN tunnel to my parents' house for 
  remote connectivity.
- **WireGuard** handles secure remote access when I'm away from home.
- **Pi-hole** runs in primary and secondary configuration for local DNS and 
  ad-blocking.
- **Active Directory** for testing domain join scenarios and group policy.

## Services

A snapshot of what's currently running:

- Auth: `authentik`, `AD`, `Vaultwarden`
- Network: `nginx-proxy-manager`, `uptime-kuma`
- Productivity: `paperless-ngx`, `actualbudget`, `hoarder`
- Media: `mealie`, `immich`
- Automation: `homeassistant`, `homebridge`
- Dev: `gitlab`, `SanbornDC`, `docker`
- Management: `proxmox`, `pbs`, `TrueNAS`, `homepage`, `pelican-panel`
- [📈 Check uptime status](https://uptime.sanborn.family/status/home) – Live view of my self-hosted services


Most services are containerized, with Docker Compose handling orchestration 
across the board.

## Goals

Right now the main project is integrating **authentik** across services and 
tying it into **Active Directory** via LDAP for centralized identity management. 
The lab is always evolving, which is the point.
