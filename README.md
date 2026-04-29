# Glance Dashboard Config

This is my personal Glance dashboard configuration for my homelab.

I’m a Mechanical Engineer getting into automation, dashboards and self-hosted tools. Not a pro developer, just building useful stuff and sharing it.

If you came here from Reddit, welcome. Take whatever is useful.

---

## Preview
**Here’s how it looks in my setup:**

> <img width="1282" height="950" alt="Glances_D (2)" src="https://github.com/user-attachments/assets/60015427-fe0a-406f-9eb4-c3d0508142cd" />


> <img width="1259" height="953" alt="Glances_D (1)" src="https://github.com/user-attachments/assets/59feb0c0-72b5-4751-a9d8-7446c47dad63" />


---

## What services am I running?

Everything runs on a **Raspberry Pi 5** with Docker. I also monitor an **Intel NUC 11** running Windows and a **VM on Google Cloud**.

| Service | Description |
|---|---|
| **Home Assistant** | Home automation |
| **Plex** | Media server |
| **Sonarr / Radarr** | TV shows and movies management |
| **qBittorrent** | Torrent client |
| **Overseerr (Seerr)** | Media requests |
| **AdGuard Home** | DNS-based ad blocking |
| **Nginx Proxy Manager** | Reverse proxy with SSL |
| **WG-Easy** | WireGuard VPN |
| **Tailscale** | Remote access |
| **Arcane** | Docker stack manager |
| **Speedtest Tracker** | Internet speed monitoring |
| **NetAlertX (Pi-Alert)** | Network device monitor |
| **Glances** | Server resource monitoring |

---

## Repository structure

```
glance-dashboard-config/
glance/
├── glance.yml         # Full Glance configuration
└── .env.example       # Required environment variables template
```

---

## How to use it

1. **Clone or download** this repository
2. Copy the `.env.example` file and rename it to `.env`:
   ```bash
   cp env.example .env
   ```
3. Edit the `.env` file and fill in your own values (IPs, passwords, API keys)
    - IP addresses
    - API keys
    - tokens
4. Use glance.yml in your setup

5. Enjoy it 😎

---

## About security

All files in this repo have been sanitized — IPs, passwords, tokens and API keys have been replaced with placeholder variables like `{{VARIABLE}}` or `${VARIABLE}`. Nothing here works as-is; you need to fill in your own values in the `.env` file.

---

## Hardware

- **Main server:** Raspberry Pi 5 (NVMe via HAT)
- **Secondary PC:** Intel NUC 11 — Windows 11
- **Cloud VM:** Google Cloud f1-micro
- **Router:** ASUS ZenWiFi AX Mini

---

## Contact

- GitHub: https://github.com/ginesjunior11
- Reddit: https://www.reddit.com/user/ginesjunior11

---

This project took time, trial and error, and a lot of learning.
I’m sharing it openly so others can use it or build on top of it.

If it helped you in any way, you can support me here:
☕ https://buymeacoffee.com/gines

No pressure, just appreciated.

[def]: <Glances_Gines (2).png>
[def2]: <Glances_Gines (1).png>
