# 🗃️ Storage Setup

My home server uses a combination of fast and redundant storage to keep things balanced and reliable:

- **Boot Drive**: Samsung Pro 990 500GB M.2 NVMe — running Proxmox VE
- **Data Storage**:
  - 2× 2TB Silicon Power SSDs in a ZFS mirror (fast storage)
  - 2× 2TB HDDs in a separate ZFS mirror (redundant bulk storage)

This layout gives me the speed benefits of SSDs for VMs and containers, while still maintaining mirrored redundancy across both sets of drives. I use Proxmox’s storage configuration options to manage both mirror pools independently.

