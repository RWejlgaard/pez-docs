# Cloudflare

I'm using Cloudflare for a few things so below I will go into detail into each service I'm using on Cloudflare.

## DNS

This is the most self-explanatory. My primary domain `pez.sh` is bought on Hover.com with the DNS servers set to those of Cloudflare.

The various subdomains are managed via [Terraform](../terraform).

## Pages

Pages is a serverless offering that will automatically deploy and serve a website from a GitHub repository.

I have it setup to listen to any commits on my [pez.sh](https://github.com/rwejlgaard/pez.sh) repository so it'll redeploy automatically.

This is also managed via [Terraform](../terraform).

## Tunnels & Zero Trust

Another great offering from Cloudflare is `cloudflared`, a tunnelling solution that makes it very easy to share HTTP services and access them through subdomains on a cloudflare managed domain.

How this works is by installing `cloudflared` onto each server and then set up "routes" that links subdomains with a port on the server. All my HTTP-enabled services are deployed this way.

"What about authorization?" I hear you say! This leads me to the Zero Trust portion of this section.

As part of Cloudflare Zero Trust, we have Cloudflare Access which provides an easy to setup authorization/login screen to services that are exposed via tunnels.

Access allows me to have all my services behind single-sign-on, or I can choose to have it disabled if I want to expose a service to anyone.

Of course this is also managed via [Terraform](../terraform).