
# opnsense-firewall-rules.md

## 🔥 Firewall Rules (Simplified)
| Interface | Source | Destination | Protocol | Action | Notes |
|-----------|--------|-------------|----------|--------|-------|
| LAN       | LAN net | any         | any      | Allow  | Allow LAN out |
| WAN       | any     | WAN address | TCP 443  | Allow  | HTTPS access |
| WAN       | any     | WAN address | TCP 22   | Block  | Block SSH access from WAN |

## 🌐 NAT Rules
- Port Forward: External WAN:8080 → Internal:192.168.1.50:80 (Web Server)

## 📡 DHCP
- 192.168.1.1 → 192.168.1.254 (Main range)
- Static: 192.168.1.10 = Home Server (Proxmox)

# 🔥 Firewall Rules (Basic Setup)

I currently have a simple set of firewall rules configured in OPNsense. These were based on a tutorial from *The Home Network Guy* and are meant to get things up and running safely while I work on tighter policies.

### Configured Zones:
- **LAN**: General internal traffic
- **WAN**: Basic external access with NAT
- **WireGuard**: VPN traffic for remote access

Right now, rules are very permissive for initial setup and testing. I plan to revisit this soon and:
- Lock down access between LAN, Guest, and IoT networks
- Add logging and monitoring to sensitive ports
- Apply tighter control to VPN connections

Stay tuned — more robust security coming soon!

