# Network
Configs for the two network segments and the router/firewall VM between them.

## Network layout
- Home network: 192.168.8.0/24 (vmbr0, Proxmox at 192.168.8.100)
- vmbr1 (servers): 10.10.10.0/24, router lab-1 ens19 
- vmbr2 (clients): 10.10.20.0/24, router lab-1 ens20 
- lab-1 ens18 = uplink on vmbr0, confirmed by MAC
