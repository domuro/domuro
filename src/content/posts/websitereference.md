+++
date = '2025-09-19T20:45:47+07:00'
draft = false
title = 'This Website'
+++
## Overview
This website is generated using [Hugo](https://gohugo.io), using the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.  It is hosted on [Vercel](https://vercel.com).

I just created this website to track some of my personal thoughts and works.

## Hugo Reference
Hugo is a tool to generate static webpages, such as this.  Following is how to create a new post.

1. Create new draft post `hugo -s src new content posts/post.md`.
2. Write post, and set `draft = false` in header.
3. Rebuild static website `hugo -s src build --cleanDestinationDir`
4. Commit and push via git
5. Validate changes on [domuro.com](https://domuro.com).  Note Vercel takes a few seconds to deploy.

## Local Testing
Local testing is accomplished via Docker.  Posts in draft will be generated on localhost.
1. `docker-compose up`
2. visit `http://localhost:1313`

## Networking Reference
* `domuro.com` domain registered via [Namecheap](https://www.namecheap.com).  
* Vercel's nameservers (ns1.vercel-dns.com, ns2.vercel-dns.com) are used to resolve this IP. 
* Vercel automatically generates (and renews) SSL certificates.  
* Vercel automatically generates ALIAS records to point `domuro.com` to domuro.vercel.app.

## Deployment
* Vercel monitors [domuro](https://github.com/domuro/domuro) GitHub repo, and automatically deploys when a commit is pushed.
