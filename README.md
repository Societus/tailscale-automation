# tailscale-automation

This repo is self-explanatory. During the process of switching from a strategy of "scaling up" to more powerful hardware, to "scaling out" to multiple hosts with low power baremetal or virtualization, I have found several things which resulted in annoying scenarios which either break things, waste time, or have no built-in way to automate when using tailscale as the primary VPN for reverse-proxying or general secure connection between hosts. So by combining existing solutions, or coming up with my own, I add them here.


So far this repo contains scripts for:

1: tailscale-cert-npm.sh - Script, systemd service, and systemd timer which will skip the maintenance period required to re-upload generated tailscale certificates into the format that Nginx Proxy Manager uses.
