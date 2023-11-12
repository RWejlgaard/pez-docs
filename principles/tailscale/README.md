# Tailscale

## Why

With my servers being on-prem that means that instead of commercial firewalls, IP routing and VPCs that's common and second nature in the cloud, I'm stuck with residential internet connections. As a principle, I don't allow incomming connections to my IP unless it's proxied.

In essence, Tailscale works like a VPC. It allows any machine or device connected to access any other machine or device.

## How

When I set up my servers, one of the first things I do is to install Tailscale and make sure it can access my other servers.

Tailscale has been so great to use that it's become the backbone of my multi-location homelab. Services like prometheus scrapes targets using Tailscale.

When I'm setting up a server I also make sure to enable "exit node" functionality, this enables the server to work as a sort of private VPN endpoint which allows me to access UK TV when in Copenhagen or the other way around.

