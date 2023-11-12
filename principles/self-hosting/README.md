# Self Hosting

## Why

I've chosen to self-host my servers as opposed to using one of numerous cloud offerings from the likes of AWS and GCP.

This boils down to one reason, recurring payment. I feel much more at ease knowing that I don't have to keep my credit-card up to date and that my servers will still be here tomorrow even if I get a new card in the mail.

This also makes it easier to expand. Sure, I could spin up a server that's equivalent to my london-b server but AWS would charge me 868 USD per month for the pleasure.

If I extrapolate that to a whole year for all my servers I have running I would be looking at a whopping 14,168 USD per year (1,180 USD per month).

It also has the side-effect that I get to have a rack cabinet in my house which brings at least some street cred when having people over.

## How

These servers were kind of free, they consist either of my old personal computers for gaming that I've repurposed into servers as I no longer have a particular interest in gaming (at least not enough to warrent a dedicated machine).

Everything I have installed on the servers is controlled and deployed via [Ansible](../ansible) so if I got a new server all I need to do is install the OS, setup SSH keys and install Tailscale. That's it, Ansible will take it from there and deploy things like node-exporter, portainer-agent and any other roles I have assigned to the specific server.