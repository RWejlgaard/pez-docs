# Terraform

## Why

Terraform is ubiquitous in todays infrastructure engineering. The ability to maintain a single source of truth for infrastructure is a crucial part of maintaining stability and "known good" configurations.

It was without even thinking about it that I chose to use Terraform for my infrastructure configuration.

I was working on setting up a few things on Cloudflare and before I knew it I had the repository [pez-terraform](https://github.com/rwejlgaard/pez-terraform) created.

## How

The repository is not very complicated. I have two things I use Terraform for right now - Cloudflare and Azure.

I made the choice not to use modules and instead opted for just having all .tf files in the root with the service prefixed (e.g "cloudflare_dns.tf").