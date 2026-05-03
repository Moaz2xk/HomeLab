# Home Server — Hardware Recovery & Build

## Overview
This project started with a dead, liquid-damaged PC (Intel Pentium Gold 
G2020, 2GB DDR3) and ended with a functional home server running 24/7. 
Everything was diagnosed, repaired, and fabricated by hand. 
No off-the-shelf solution.

## Hardware
- Intel Pentium Gold G2020
- Diagnosed and repaired liquid damage
- Destroyed power system fully rewired
- Hardware kill switch added to power circuit
- Custom control panel fabricated — indicator LEDs and switches 
  mounted on drilled chassis
- TP-Link POE adapter on top panel
- Colour-coded ethernet cables

## Phase 1 — pfSense
<img width="783" height="391" alt="images (8)" src="https://github.com/user-attachments/assets/dd3424bf-fbbc-499e-9137-42cd18a70cbc" />

Running pfSense as the primary OS for network management:
- Site blocking and content filtering
- Traffic monitoring
- QoS bandwidth control per device using qband

## Phase 2 — TrueNAS scale (Current)
<img width="1280" height="623" alt="1703668902825" src="https://github.com/user-attachments/assets/3a56daad-2244-481f-af0a-a4774e693f9e" />

Switched to TrueNAS bare metal when pfSense no longer met storage needs:
- **TrueNAS** — bare metal NAS OS with ZFS storage
- **SMB shares** — shared storage across Windows, laptop, and mobile
- **Jellyfin** — self-hosted media server
- **Tailscale** — VPN for remote access

## What I Learned
- Hardware fault diagnosis on liquid-damaged boards
- Power circuit design and rewiring
- pfSense firewall rules, traffic monitoring, and QoS configuration
- TrueNAS ZFS pool setup and management
- SMB network share configuration
- Self-hosted media server setup
- Remote access via Tailscale VPN

## Documentation
- Build photos
- Wiring diagrams
- Control panel fabrication notes
