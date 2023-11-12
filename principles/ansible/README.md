# Ansible

## Why

As I've detailed in the section about [self-hosting](../self-hosting). I'm running all my infrastructure on-prem which means a lot of the little automations and the mindset of "just spin up a new machine" does not apply to my situation.

This means that instead of being "cattle" my servers are more like pets.
Being from a sysadmin-ish background, this is no bueno.

I want to handle my "pets" as much like cattle as possible so everything I deploy to them is via Ansible. This means that if disaster strikes and let's say, I lose a disk or something I can get up and running in about 30 minutes give and take.

## How

My repo titled [pez-ansible](https://github.com/rwejlgaard/pez-ansible) contains all the roles of my servers divided up into each location.

These roles are applied via GitHub Actions every time I commit to the master branch. This automated deployment has been a life-saver a couple times when I'm out and about and something is misconfigured. All I have to do is a quick commit from my phone.

Ansible works via SSH and for security reasons I don't expose my SSH ports on my network to the internet. So these SSH connections are done via [Tailscale](../tailscale).

The role definitions are done in a global `site.yml` file that's run via the pipeline.