# My Resume

<a href="/mitchell-sanborn-resume.pdf" target="_blank" rel="noopener">📄 Download Resume</a>

# Beyond the Resume

A resume is a summary, not the whole picture. This is where I keep the rest: the projects, the philosophy, and the things I've learned from doing this work for a while.

---

## 🧠 How I Think About IT

**IT should feel personal.** Users deserve support that actually listens and adapts to how they work, not just how the system was designed.

**Documentation is part of the deliverable.** I write things down clearly and with context. Good docs keep systems resilient and make handoffs smoother for whoever comes next.

**Simple beats clever.** A stable, well-supported solution beats something complex that only one person can maintain.

**Test first, then deploy.** The homelab exists to break things safely before they hit production. It has saved me from more than a few disasters.

**Respect the user's workflow.** Every environment is different. The goal is to enhance how people work, not force them into new habits to fit a system.

---

## 🛠️ Projects I Couldn’t Fit on My Resume

**AD and DNS rebuild with zero downtime.** Took aging, unreliable domain infrastructure and rebuilt it on Proxmox using repurposed hardware. Deployed a clean Windows Server instance in our Salt Lake office, migrated roles and services, and established replication with the secondary site without any end-user disruption. Cleaned up outdated policies and simplified DNS zones in the process.

**Brewery PCI network design.** Designed a secure, segmented network for a local brewery including POS isolation, guest Wi-Fi, camera VLANs, and a site-to-site VPN. Replaced unmanaged legacy hardware with modern VLAN-capable gear and got the final design through a third-party PCI audit.

**Onboarding without the ticket queue.** Replaced a fragmented onboarding process with a straightforward workflow built around real communication instead of automated ticket chains. Result: consistent device setup, smoother user transitions, and less back-and-forth with HR.

**Self-hosted infrastructure.** The homelab runs 30-plus services covering everything from file storage to security tooling, structured to mirror real client environments so I can test updates and configuration changes with zero production risk.

---

## 🔍 Things I’m Digging Into

**SSO via Authentik and Active Directory.** Mid-rollout on integrating Authentik cross lab services with LDAP to centralize identity management, with the longer goal of bringing this to clients who need better access control.

**Onboarding automation.** Writing PowerShell and Bash scripts to make user setup, permissions, and device configuration a one-step process instead of a checklist.

**Proxmox and TrueNAS workflows.** Working on tighter integration between the two for shared storage and backup consistency across VMs and containers.

---

## ⚙️ Tools I Really Like

**Proxmox.** My go-to for virtualization. Stable, flexible, and works well on older hardware.

**Jamf, Addigy, and Intune.** The right way to manage Apple and Windows devices at scale, especially in BYOD and education environments.

**Docker and Compose.** Lightweight, portable, and works equally well in a homelab and a production environment.

**UniFi.** Easy to manage, VLAN-friendly, and the full stack (Network, Access, Protect, Talk) covers most of what a small-to-mid organization actually needs.

**Markdown and Wiki.js.** Clear, maintainable documentation is half the battle in IT. These make it easier to actually write it.

---

## 🤓 Fun (Or Painful) Quirks

I color-code patch cables. It's equal parts aesthetic and sanity.

I use OneNote for time tracking, not because it's the best tool for it, but because it creates clear accountability. It shows what was done, how long it took, and leaves enough context for the next person to understand how things were set up.

My homelab's uptime has outperformed some production networks I've inherited. 

I'll leave it at that.