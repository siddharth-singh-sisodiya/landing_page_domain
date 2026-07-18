# Coming Soon

A single-page "coming soon" placeholder site, ready to deploy to GitHub Pages (or any static host).

## Preview

A centered vintage-inspection-style badge — an owl perched on a fire extinguisher — with a "Coming Soon" headline underneath.

## Deploying with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder.
4. Save. Your site will be live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Using a custom domain

1. In **Settings → Pages**, enter your domain under **Custom domain** (this creates a `CNAME` file in the repo automatically — or add one yourself containing just your domain name, e.g. `example.com`).
2. At your domain registrar, point DNS at GitHub Pages:
   - For an apex domain (`example.com`): add `A` records pointing to
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - For a subdomain (`www.example.com`): add a `CNAME` record pointing to `<your-username>.github.io`
3. Wait for DNS to propagate, then enable **Enforce HTTPS** in the Pages settings once available.

## Local preview

Just open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Structure

```
.
├── index.html   # the entire site
├── README.md
└── LICENSE
```

No build step, no dependencies beyond a Google Fonts CDN link (with system-font fallbacks if that's unreachable).
