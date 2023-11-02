# boltauthd
## Installation
Copy [boltauthd](./boltauthd) and [boltauthd-boltctl-integration](./boltauthd-boltctl-integration) both /usr/bin/

Then start the background service

### OpenRC
Copy [boltauthd](./boltauthd-openrc) to /etc/init.d/boltauthd and add the service to the default runlevel
```
sudo rc-update add boltauthd default
```

Restart your system and alias boltctl to boltauthd-boltctl-integration to automatically list PCI IDs in the output next to each Thunderbolt device ID
