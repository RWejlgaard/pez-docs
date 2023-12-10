# Plex

## History

My Plex server is what started my homelab. I had two 3 TB drives laying around so I thought I should try out setting up a plex server.

This was hosted on a single Proxmox server on the hardware that would later turn into `london-a`. I thought I was being smart about the way I had it set up, using seperate VMs for each function of the setup with a VM serving the central storage over NFS.

I hadn't thought about the limitations of NFS when I set it up and I would often find that if I was downloading media while streaming I would reach the limits of NFS I/O.

Once I got hold of 3 new hard drives of 8 TBs (24 TB striped capacity). I bit the bullet and installed the OS on the bare metal which leads us to the current setup.

## Current Setup

My current plex setup is running on my `london-b` server. The server is rediculously overpowered as a media server, it's equipped with a Threadripper CPU and an Nvidia GTX 980.

The GPU helps a bit with transcoding while streaming but the CPU can easily transcode plenty fast by itself.

The storage is directly attached to the motherboard and my three 8 TB drives are striped to maximize the usable storage. I don't really care if I loose a disk, since it's only movies and TV shows anyway. Although, it would suck having to re-download everything.

I use the so-called `*arr` stack. Radarr, Sonarr & Prowlarr for movies, TV shows and trackers respectively.

For my download client I first went with Deluge which I **not** like. It was slow and sluggish, constantly corrupting downloads and not cleaning up after itself.

So I'm now using Transmission, which is brilliant. It's so good I'm able to have 100 active torrents at once!

## Future upgrades

I'm planning a rather large purchase to expand my raid array with 21 additional disks which would bring my total capacity to 192 TB (this will not be striped).