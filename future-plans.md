
# 🧠 Future Plans – Bearded Pixels Home Server

This system is just getting started! Here’s what I plan to expand into soon:

---

## 🛠️ Networking

- 🔲 Implement VLANs to separate devices (IoT, personal, guest, servers)
- 🚦 Advanced OPNsense firewall rules for tighter security
- 🌍 Set up Dynamic DNS for remote access
- 🟢 Expand WireGuard access control lists for more fine-tuned remote access
- 📱 Add a killswitch and auto-connect on mobile clients
- 🔐 Enable MFA and better logs for VPN sessions

---

## 💾 Storage

- 🗃️ Add ZFS for better redundancy and snapshot support
- ☁️ Integrate Proxmox backup server or use TrueNAS as NFS target
- 🔁 Automate document syncing from my main devices

---

## 📦 Self-Hosted Apps (On Proxmox Containers/VMs)

- 📚 [ ] Paperless-NGX for document management  
- 💸 [ ] Firefly III for personal finance tracking  
- 📡 [ ] Pi-hole for network-wide ad-blocking  
- 🧪 [ ] GitLab or Gitea for code hosting  
- 🌐 [ ] Nextcloud for private cloud storage  

---

## 🧰 System Monitoring

- 📊 Add Grafana + Prometheus (or Netdata) for real-time metrics
- 🔔 Set up health alerts (e.g., disk failure, high temps)

---

## 🪪 Security

- 🔐 Harden SSH (keys only, no password)
- 🚫 Block unused ports and create geo-IP rules in OPNsense
- 🧱 Regular firewall config exports with Git tracking
