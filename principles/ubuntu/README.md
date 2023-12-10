# Ubuntu

## History

The path to choosing Ubuntu as my primary OS was a long journey.

### Proxmox

Originally when my homelab was just getting started I wanted to run everything as a VM or a container.
I found out eventually that Proxmox just didn't fit me, it's a long story that I won't go into in this section but long story short - I found Proxmox to be sluggish, resource inefficient, infuriating and hard to maintain.

On my Proxmox I used a bunch of different distros, primarily a very slim version of Debian 12 since I wanted the OS to be super lightweight.

This lead me to instead use Alpine Linux on my VMs and containers instead of Debian and I chose Alpine when I eventually torched my Proxmox installation and went bare metal.

### Alpine Linux

I still love Alpine, it's blazing fast and uses minimal resources on the machine.

I timed myself how fast I could run through the installer for Alpine from boot to fully configured machine and I clocked in at just under 5 minutes. 

There's something about Alpine that makes everything feel instantaneous.

### Ubuntu (current setup)

As much as I love Alpine, I setup Ansible on my servers and I kept getting issues with Alpine since it's a _special_ distribution.

The lack of GNU binaries and systemd eventually got to me enough that I switched to Ubuntu.

I don't really like Ubuntu, install process takes at least 15 minutes, updates take forever to install and it keeps wanting me to reboot my servers but it's well supported by Ansible and the various roles I'm using.

