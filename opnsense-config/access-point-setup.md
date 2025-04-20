# 🌐 Access Point (AP) Setup

For wireless networking, I repurposed an old TP-Link router and configured it as a dedicated access point. Here's how I set it up:

- Logged into the TP-Link admin interface
- Enabled **Access Point Mode**
- Configured the following networks:
  - 5GHz and 2.4GHz main Wi-Fi
  - Guest Network
  - IoT Network
- Connected it directly to the switch, which is then uplinked to my OPNsense firewall

This setup gives me flexible wireless access across multiple isolated networks, ready for VLANs or firewall segmentation later on.

