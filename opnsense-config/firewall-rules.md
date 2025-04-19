
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
