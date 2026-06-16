# Homelab

Personal homelab running on a Synology NAS with Docker-based services
for media management and network-level ad blocking.

## Hardware
- **NAS:** Synology DS918+ — 40TB usable storage
- **Other:** Raspberry Pi 3 (Pi-hole)

## Services
| Service | Purpose | Hosted On |
|--------|---------|-----------|
| Plex | Media server | Synology (Docker) |
| Radarr | Movie management | Synology (Docker) |
| Sonarr | TV management | Synology (Docker) |
| Prowlarr | Indexer manager | Synology (Docker) |
| Pi-hole | Network ad blocking | Raspberry Pi 3 |

## Data Structure
- `data/media/` — books, movies, music, tv
- `data/torrents/` — torrent downloads
- `data/usenet/` — usenet downloads
- `docker/` — per-service Docker config folders

## Repo Structure
- `/media` — Docker Compose and env template for the full stack
- `/nas` — Synology scripts and scheduled tasks
- `/pihole` — Pi-hole configuration and blocklists

## Notes
VPN routing handled via Gluetun container.
