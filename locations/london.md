# London

This location is my primary one. It's hosted at my address in northwest London in my rack cabinet in my bedroom (doubles as a white noise machine for falling asleep).

It consists of 3 servers, A,B and C. 

A and B are my old personal computers but since I don't play that many games anymore the servers are now retired into the coal mine that is their duty as servers.

The "C" server is a raspberry pi 4. I plan to replace this once raspberry pi 5's become generally available. As well as increase the amount to fill out the 1U of rack space that can contain up to 4 Pi's.

## Networking

Networking is fairly overkill I have to admit. I'm using a Ubiquiti Dream Machine Special Edition as my router which gives my excellent routing performance compared to a normal ISP-provided router.

My ISP (BT) are charging me about £90 for a 1Gbit/300Mbit connection. This connection is fine, latency is a tad high at times for a supposedly "fiber" link.

I've been pretty lucky that my flat is equipped with Cat 5 cabling in the walls which is accessible via a patch panel in my utility closet. All cables in the wall are connected to a Ubiquiti switch which is mounted onto the wall of the closet.

## Other bits

I was getting fed up having to load up grafana on my devices just to have a quick glance to check if all is doing okay so I invested in a refurbished tablet that I've stuck onto the side of my fridge in my living room. This way, I can sit in the couch and glance at various dashboards.

## Hardware Specs

### london-a

|Component|Value|
|---|---|
|CPU|Intel i7 4790K|
|vCPUs|8|
|Memory|32 GB|
|GPU|On-board CPU|
|Boot Storage|1 TB|
|Extra Storage|N/A|

### london-b

|Component|Value|
|---|---|
|CPU|Threadripper 3970X|
|vCPUs|64|
|Memory|64 GB|
|GPU|Nvidia GTX 980|
|Boot Storage|500 GB|
|Extra Storage|96 TB|

### london-c

|Component|Value|
|---|---|
|CPU|ARM Cortex-A72|
|vCPUs|4|
|Memory|8 GB|
|GPU|On-board CPU|
|Boot Storage|128 GB|
|Extra Storage|N/A|
