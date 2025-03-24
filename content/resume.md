# My Resume

<a href="/mitchell-sanborn-resume.pdf" target="_blank" rel="noopener">📄 Download Resume</a>

# Off-Resume Things

There’s only so much you can cram into a single page of a resume. This is where I keep the rest — the stories, philosophies, and hands-on wins that reflect how I actually work, not just what tools I’ve used.

---

## 🧠 How I Think About IT

- **IT should be personal.** I believe users deserve support that feels human. That means listening, tailoring solutions, and not hiding behind tickets or buzzwords.
- **Documentation is part of the deliverable.** I write things down — clearly and with context. Good documentation keeps systems resilient and makes handoffs smoother for everyone involved.
- **Simple beats clever.** I’d rather deploy something stable and well-supported than something overly complex that only I can fix.
- **Test first, then deploy.** My homelab exists to break things safely before they hit production. It’s saved me (and clients) from disaster more than once.
- **Respect the user's workflow.** Every environment is different. My goal is to enhance how people work, not force them into new habits just to fit a system.

---

## 🛠️ Projects I Couldn’t Fit on My Resume

- **AD + DNS rebuild with zero downtime:** Took aging, unreliable domain infrastructure and rebuilt it using Proxmox on repurposed hardware. I deployed a clean Windows Server instance in our Salt Lake office, migrated roles and services, and established replication with the Murray site — all without end-user disruption. Bonus: cleaned up outdated policies and simplified DNS zones in the process.
- **Brewery PCI network design:** Created a secure, segmented network for a local brewery including POS isolation, guest Wi-Fi, camera VLANs, and a secure site-to-site VPN. The project involved replacing unmanaged legacy hardware with modern, VLAN-capable gear and ensuring the final design passed a third-party PCI audit.
- **Onboarding, without the tickets:** Replaced a jumbled onboarding process with a straightforward workflow that relies on real communication instead of automated ticket queues. The result: consistent device setup, smoother user transitions, and less back-and-forth with HR.
- **Self-hosted playground:** My homelab runs over 30 services — everything from file servers to security tools — mimicking client environments so I can test updates, configuration changes, and integrations with zero risk.

---

## 🔍 Things I’m Digging Into

- **SSO via Authentik + Active Directory:** I’m mid-way through rolling out Authentik across my services with LDAP integration to centralize login management and eventually bring this to clients who need better identity control.
- **Onboarding automation:** Writing PowerShell and Bash scripts that make user setup, permissions, and device configuration less of a chore and more of a one-click process.
- **Proxmox + TrueNAS workflows:** Working on making the two coexist more elegantly for lab backups and shared storage across VMs and containers.

---

## ⚙️ Tools I Really Like

- **Proxmox** – My go-to for virtualization. Stable, flexible, and friendly to older hardware.
- **Jamf + Mosyle** – Essential for managing Apple devices the right way, especially in BYOD and education settings.
- **Docker + Compose** – Lightweight service deployment that’s perfect for both homelab tinkering and real client use cases.
- **UniFi gear** – Easy to manage and VLAN-friendly, with just enough nerd knobs to keep things interesting.
- **Markdown + Wiki.js** – Clear, fast, and maintainable documentation is half the battle in IT.

---

## 🤓 Fun (Or Painful) Quirks

- I color-code patch cables for aesthetic *and* sanity.
- I still use OneNote for time tracking — not because it's perfect, but because it creates clear accountability for clients. It shows what I did, how long it took, and leaves a trail of notes for the next tech to understand how things were set up.
- My homelab's uptime has outperformed some production networks I’ve inherited (not naming names).