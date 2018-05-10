---
layout: post
title: Custom domain with github
---
[Freenom](https://www.freenom.com) allows to register custom domain for free for 12 months with ending *.tk *.ml *.ga etc. Github allows to host static
pages and register them within custom domain e.g. `myexample.tk` and `www.myexample.tk`. The following instruction shows how to do that. 

## Free custom domain

[Freenom](https://www.freenom.com) allows to register custom domain for free for 12 months with ending *.tk *.ml *.ga etc.
Register e.g. with google account and choose/register available domain for free e.g. `myexample.tk`.

## Github pages

Within a project you may create github pages (master branch or special gh-pages branch).
- Select your project in Github https://github.com/<your name>/<yourproject>
- Go to Settings
- Scroll to Github pages (optionally select Source and Theme Changer)
- Fill custom domain, e.g. `myexample.tk`

## Freenom A record

Now you need to register A records within your domain at freenom

First to enable it, follow STEP 1 and then STEP 2 to configure 

- STEP 1
-- Go to My Domains
-- Click on Manage Domain
-- Click on Management Tools
-- Click on Nameservers
-- Select Use default nameservers
-- Press Change Nameservers, DONE!
- STEP 2
-- Click on Manage Domain
-- Manage Freenom DNS
-- Now you can enter a variety of different DNS records, including A, MX and CNAME records.
- STEP 3
-- register these A records (current instructions at [help.github.com](https://help.github.com/articles/setting-up-an-apex-domain/) )
--- 185.199.108.153
--- 185.199.109.153
--- 185.199.110.153
--- 185.199.111.153
These may take up to 30 minutes to be propagated through Internet. 

## Freenom CNAME record

if you want `www` subdomain to be handled by the same web pages, register CNAME record
-- Go to My Domains
-- Click on Manage Domain
-- Manage Freenom DNS
-- Add CNAME with Name `www` and target `<your name>.github.com`
This may take up to a day to be propagated through Internet.
 