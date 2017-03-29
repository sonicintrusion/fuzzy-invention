1. Must copy the authorized_keys file into place
2. Hostname must be set manually (for now)
3. NTP server must be built first
4. DHCP server needs to be built before the other regular servers
5. DHCP server must have static IP address

Roles working:
- bastion (ssh)
- common (all servers except ntp server)
- dhcp (server)
- dns (server)
- ntp (server)
- vpn (l2tp server) -- must run ask-vault-pass switch when running playbook

Roles need doing:
- adblock (pi-hole)
- downloader (sabnzbd)
