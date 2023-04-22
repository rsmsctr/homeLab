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

    Truenas for file hosting via SMB, Proxmox Backups, and Veeam Agent backups

    Proxmox with 2 Ubuntu Server VM's | Ubuntu Server with Docker running a Plex media application stack | Ubuntu Server running TP-Link Omada SDN Software

    Raspberry Pi running Tailscale

    Ubuntu Server with Docker running Pi-hole and a Discord bot

