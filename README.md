# Home Lab
![networkdiagram(7)](https://user-images.githubusercontent.com/95463866/233758211-da3f989f-9e4d-4f4b-917f-a5fef2e2dd8e.jpg)


Hello and thank you for checking out my homelab! 

Two VLANS:

VLAN1 - LAN

VLAN50 - WorkLAN



Two SSID's:

Personal - VLAN1

Work - VLAN50



ACL rules are set to block communication between both LAN's on all ports.

VLAN1 Hosts:

    TrueNAS host for file hosting via SMB, Proxmox Backups, and Veeam Agent backups

    Proxmox host with 2 Ubuntu Server VM's | Ubuntu Server with Docker running a Plex Media Application Stack | Ubuntu Server running TP-Link Omada SDN Software
    
        Plex Media Application Stack:
            -Sonarr - TV Collection Manager
            -Radarr - Movie Collection Manager
            -Jackett - Proxy server to translate tracker site specific http queries
            -Gluetun - VPN Container - Other containers within the application stack are bound and routed through this containers network
            -Plex - Video streaming service
       
    Raspberry Pi host running Tailscale within Ubuntu Server

    HP Host running Ubuntu Server with Docker running Pi-hole DNS server and a Discord bot

