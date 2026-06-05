# Homelab

Personal homelab running on a Synology NAS with Docker-based services
for media management and network-level ad blocking.

## Hardware
- **NAS:** Synology [model] — [X]TB usable storage
- **Network:** [router/switch if worth mentioning]
- **Other:** Raspberry Pi 3 (Pi-hole)

## Services
| Service | Purpose | Hosted On |
|--------|---------|-----------|
| Plex | Media server | Synology (Docker) |
| Radarr | Movie management | Synology (Docker) |
| Sonarr | TV management | Synology (Docker) |
| Prowlarr | Indexer manager | Synology (Docker) |
| Pi-hole | Network ad blocking | Raspberry Pi 3 |

## Structure
- `/media` — Docker Compose and config for the full media stack
- `/nas` — Synology scripts and scheduled tasks
- `/pihole` — Pi-hole configuration and blocklists

## Notes
Any quirks, lessons learned, or setup decisions worth documenting.
