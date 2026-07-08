#VPS-Kamatera

A self-managed VPS used to run VPN and file-sync services, set up to get around port restrictions in my dorm's network.

Demo

https://www.youtube.com/watch?v=0Txh8oTFT4c

Setup


Provider: Kamatera
OS: Ubuntu LTS 24
Firewall: UFW, with only the necessary ports open:

22/tcp - SSH
51821/udp - WireGuard
1194 - OpenVPN


Services running:

WireGuard
OpenVPN
Nextcloud



Why This Exists

My dorm's network blocks incoming ports, which makes self-hosting anything reachable from outside pretty much impossible. Renting a VPS with a public IP and no such restrictions let me run a VPN back into my own setup and self-host file sync (Nextcloud) without depending on the dorm's network limitations.

Why I Stopped

The VPS's network speed was too slow to comfortably run everything I wanted on it. So I stopped renewing the subscription and I'm now using the Pi Keeper for the same purposes.



Tech Stack

Ubuntu LTS 24
Nextcloud
UFW
WireGuard, OpenVPN
Nextcloud
UFW
