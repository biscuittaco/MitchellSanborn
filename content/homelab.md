# Homelab

Welcome to the Sanborn Homelab — part testing ground, part personal infrastructure, and part proving ground for projects I might roll out to clients. It’s where I experiment, break things on purpose, and keep the gears turning at home.

## Hardware

The lab is currently spread across three primary systems:

- **Custom-built PC** with a Ryzen 7 3700x and 32GB of RAM — used for lightweight workloads and Docker containers.
- **Dual-node Supermicro SYS-2028TP-DC1R** — each node runs dual Xeon E5-2643 v4 CPUs and 128GB of RAM. This is where most of the heavy lifting happens.
- **TrueNAS server** for storage, served over NFS and used as a Proxmox Backup target among other things.

## Networking

The network is managed through a **UniFi Dream Machine Pro**. Everything is segmented with VLANs for isolation and clarity. I use:

- **Site Magic** to maintain a VPN tunnel between my house and my parents’ for remote connectivity.
- **WireGuard** for secure remote access when I’m away from home.
- **Pi-hole (primary + secondary)** for local DNS and ad-blocking.
- **Active Directory** to test domain join scenarios and group policy application.

## Services

Here are just a few of the services currently running across the lab:

- Auth: `authentik`, `AD`, `Vaultwarden`
- Network: `nginx-proxy-manager`, `uptime-kuma`
- Productivity: `paperless-ngx`, `actualbudget`, `hoarder`
- Media: `mealie`, `immich`
- Automation: `homeassistant`, `homebridge`
- Dev: `gitlab`, `SanbornDC`, `docker`
- Management: `proxmox`, `pbs (Proxmox Backup Server)`, `TrueNAS`, `homepage`, `pelican-panel`

Everything’s containerized where possible, with Docker and Compose managing a good chunk of the orchestration.

## Automation & Backups

I’ve used resources like [Helper-Scripts.com](https://helper-scripts.com), but much of the setup has been done manually to better understand the ins and outs. Proxmox handles backups with its native backup server, writing to TrueNAS over NFS.

## Goals

The lab doesn’t follow a strict philosophy—just solid performance to support testing, learning, and real-world reliability. Right now, I’m working on integrating **authentik** across most services and tying it to my **Active Directory** for centralized identity via LDAP.

It's always evolving, and that’s the fun part.
