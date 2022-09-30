# homelab
Configurations for my homelab


## Steps for setup

- Configure Adguard Home as local DNS
  - Set mydomain.com and subdomains thereof to point to traefik server
- Set router to point to Adguard Home
- Setup Traefik and other Stacks

## Hosts

### Docker environments

| IP            | ID  | Name      | Notes                                                      |
|:--------------|:----|:----------|:-----------------------------------------------------------|
| 192.168.1.200 | N/A | adguard   | Local DNS w/ dns-wide ad-blocking                          |
| 192.168.1.201 | N/A | proxmox   | KVM hypervisor (main node)                                 |
| 192.168.1.202 | 102 | traefik   | Reverse proxy & load balancer                              |
| 192.168.1.203 | 103 | vpn       | Local VPN access w/ Wireguard                              |
| 192.168.1.204 | 104 | portainer | Container management interface                             |
| 192.168.1.205 | 105 | dash      | Homelab dashboard for quick-access                         |
| 192.168.1.206 | 106 | wiki      | Homelab wiki                                               |
| 192.168.1.207 | 107 | rss       | Personal RSS feed                                          |
| 192.168.1.208 | 108 | bitwarden | Password manager w/ vaultwarden                            |
| 192.168.1.209 | 109 | vscode    | Visual Studio Code in the browser                          |
| 192.168.1.210 | 110 | status    | Monitor server status w/ Netdata, Prometheus & Grafana     |
| 192.168.1.211 | 111 |
| 192.168.1.212 | 112 |
| 192.168.1.213 | 113 |
| 192.168.1.214 | 114 |
| 192.168.1.215 | 115 |
| 192.168.1.216 | 116 |
| 192.168.1.217 | 117 |
| 192.168.1.218 | 118 |
| 192.168.1.219 | 119 |
| 192.168.1.220 | 120 |

## Deployment checklist

- [ ] Change hostname with sudo hostname ${HOSTNAME}
- [ ] Change default password ("changeme") with passwd
- [ ] Set static IP with netplan @ /etc/netplan/..

