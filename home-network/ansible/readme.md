# Sets up home network infrastructre

## Reqs

1. Must have a private key stored in the /.ssh/ directory
1. Must copy the authorized_keys file into place on each server
1. Hostname must be set manually (for now)
1. NTP server must be built first
1. DHCP server needs to be built before the other regular servers
1. DHCP server must have static IP address

## Current status

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
