# lvm.me

My personal blog. Built with Hugo, custom terminal theme, auto-syncs from Notion, deploys to Cloudflare Workers.

## 📁 Project Structure

```
├── hugo.yaml              # Main Hugo configuration
├── wrangler.jsonc          # Cloudflare Workers configuration
├── render.yaml             # Notion to Hugo content rendering rules
├── content/                # Blog content (auto-generated from Notion)
├── public/                 # Generated static site
├── themes/my-terminal/     # Custom terminal theme
├── resources/              # Hugo generated resources
└── .github/workflows/      # CI/CD automation
    └── deploy.yaml
```

## Setup

```bash
# Run locally
hugo server -D

# Build
hugo --minify
```

## Deploy

Syncs from Notion daily via GitHub Actions. Deploys to Cloudflare Workers.