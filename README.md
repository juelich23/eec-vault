# EEC Vault

Static one-page site for EEC Vault (Eggeggchicken Vault), a sports card
dealership based in Los Angeles, California.

Live at https://eecvault.com/

## Structure

    index.html      the whole site - no build step, no JavaScript
    assets/         card photographs
    favicon.svg     slab-and-card mark

Everything is plain HTML and CSS. Open `index.html` in a browser to preview,
or serve the folder:

    python3 -m http.server 8000

## Deploying

Pushing to `main` publishes automatically via GitHub Pages.

## Custom domain

`eecvault.com`, registered at Cloudflare. DNS is four apex A records
pointing at GitHub Pages plus a `www` CNAME, all set to DNS-only (not
proxied) so GitHub can issue the TLS certificate. The `CNAME` file in
this repo is what tells Pages which domain to serve.
