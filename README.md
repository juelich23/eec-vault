# EEC Vault

Static one-page site for EEC Vault (Eggeggchicken Vault), a sports card
dealership based in Orange, California.

## Structure

    index.html      the whole site - no build step, no JavaScript
    assets/         card photographs
    favicon.svg     slab-and-card mark

Everything is plain HTML and CSS. Open `index.html` in a browser to preview,
or serve the folder:

    python3 -m http.server 8000

## Deploying

Pushing to `main` publishes automatically via GitHub Pages.

## Still to fill in

- `Years in operation` and `Shows attended per year` are marked *Pending*
  in the Record section.
- `REPLACE-WITH-YOUR-DOMAIN` appears in the canonical and og:image tags in
  `index.html`. Replace both once a custom domain is pointed here, otherwise
  link previews will not render.

## Custom domain

Add a `CNAME` file containing the bare domain, then point DNS at
GitHub Pages. Update the two meta tags above at the same time.
