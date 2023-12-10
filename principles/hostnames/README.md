# Hostnames

## History

For my setups in my locations, I decided to use a simple "A, B, C" approach since the amount of servers I have in posession is quite small compared to setups that are running in private clouds such as AWS or GCP.

I'm _unlikely_ to have more than 26 servers in one location. (and if I do I should probably go touch some grass).

## Problem

This "ABC" scheme had served me well for over a year but it felt very clinical to SSH into "{location}-a".

I realized that I missed the fun of actually naming a server. When a server has a real human names, suddenly they take on a personality.
If a server is being difficult when rolling out a deployment, it's fun to think "Oh that's good ol' Betsy having a moment".

## Solution

What I ended up with is to still use names such as "copenhagen-a" as a primary hostname with services such as prometheus and tailscale referencing that name to keep configs simple and readable.

However, I set the actual hostname on the machines to include a name starting with the letter of the server that is local to the geographical location. In copenhagen-a's case that would be "copenhagen-aksel".

This makes them way more fun to play around with. The names being local to the geographical area make them feel unique.