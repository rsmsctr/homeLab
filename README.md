# Home Lab
![networkdiagram(7)(7) drawio](https://user-images.githubusercontent.com/95463866/234155553-7db73a89-5361-4aab-b946-e296806cfcc0.png)



Two VLANS:

    VLAN1 - LAN - 192.168.0.1/24
    VLAN50 - WorkLAN - 192.168.50.1/24



Two SSID's:

    Personal - VLAN1
    Work - VLAN50



ACL rules are set to block communication between both LAN's on all ports.

VLAN1 Hosts:

    TrueNAS host for file hosting via SMB, Proxmox Backups, and Veeam Agent backups

    Proxmox host with 2 Ubuntu Server VM's: Ubuntu Server with Docker running a Plex Media Application Stack | Ubuntu Server running TP-Link Omada SDN Software
    
        Plex Media Application Stack:
            Plex
            Docker:
                -gluetun(1) - VPN Container
                -sonarr(2)
                -radarr(3)
                -jackett(4)
                -qbittorrent(5)
       
    Raspberry Pi host running Ubuntu Server: Tailscale

    HP Host running Ubuntu Server with Docker: Pi-hole DNS server | Discord bot

