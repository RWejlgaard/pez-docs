# Copenhagen

This location is self-hosted and serves as my secondary location. The main firepower is located in London.

I've set up a stack of servers at my Dad's place to work as an off-site location. These servers are not super powerful but they're excellent for hosting services that require a static IP since my ISP in London likes to charge for that privilege.

At this location I have 3 servers setup, A, B and C. A and B are Lenovo "tiny" desktop computers. I really like these boxes. They're very compact at about the size of a lunchbox and power is provided via a normal ThinkPad charging brick. The last server is a Raspberry Pi 4.

## Networking

There's not much to talk about here. Since it's not my house I'm not really at liberty to install a balls-to-the-wall networking setup. So I'm using the ISP provided router with each of the 3 servers connected directly to the built in switch in the router.

The connection is a symmetrical 500 Mbit. Plenty for hosting a few websites or other smaller services.

## Hardware Specs

### copenhagen-a

|Component|Value|
|---|---|
|CPU|Intel i5 4570T|
|vCPUs|4|
|Memory|6 GB|
|GPU|On-board CPU|
|Boot Storage|500 GB|
|Extra Storage|N/A|

### copenhagen-b

|Component|Value|
|---|---|
|CPU|Intel i5 4570T|
|vCPUs|4|
|Memory|6 GB|
|GPU|On-board CPU|
|Boot Storage|500 GB|
|Extra Storage|N/A|

### copenhagen-c

|Component|Value|
|---|---|
|CPU|ARM Cortex-A72|
|vCPUs|4|
|Memory|8 GB|
|GPU|On-board CPU|
|Boot Storage|128 GB|
|Extra Storage|N/A|