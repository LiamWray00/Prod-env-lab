# Change log

## 2026-11-22
- Created Proxmox bridges vmbr1 (servers) and vmbr2 (clients), no physical ports
- Snapshot lab-1 "before-router"
- Added net1 (vmbr1) and net2 (vmbr2) to lab-1
- Next: static IPs on ens19/ens20, enable IP forwarding

## 2026-11-23
- Snapshot lab-1 "before-static-ips"
- Assigned router interfaces 10.10.10.1/24 (ens19, servers) and 10.10.20.1/24 (ens20, clients) via /etc/netplan/60-lab.yaml
- Enabled IP forwarding via /etc/sysctl.d/99-forwarding.conf
- Issue: ip_forward stayed 0 because the key inside the conf file was misspelled; fixed and verified = 1
- Next: move lab-2 onto vmbr2 and test routing
