# Dragon Testing — US site

Single-page static site for the US market. No build step: plain HTML + CSS, assets in `assets/`.
Same structure as `llmtestlabs-site`.

## Local preview

    python3 -m http.server 8000

## Deploy (GitHub Pages)

1. Create the repo on GitHub (e.g. `longce/dragontesting-us-site`) and push this folder to `main`.
2. Settings → Pages → Source: **Deploy from a branch** → `main` / `(root)`.
3. Custom domain: add a `CNAME` file containing the domain (e.g. `dragontesting.ai`),
   then in Cloudflare DNS add a CNAME record for the domain pointing to `longce.github.io`
   (DNS only / grey cloud until GitHub issues the certificate), and tick "Enforce HTTPS".
