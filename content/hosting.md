---
title: Hosting
---

Quartz generates static HTML, CSS, and JavaScript files that can be hosted on any web server. Here are some popular hosting options.

## Vercel

1. Connect your GitHub repository to Vercel
2. Set build command to: `npm run build`
3. Set output directory to: `public`
4. Deploy!

## Netlify

1. Connect your GitHub repository to Netlify
2. Set build command to: `npm run build`
3. Set publish directory to: `public`
4. Deploy!

## GitHub Pages

Create a GitHub Actions workflow to automatically build and deploy:

```yaml
name: Deploy Quartz site to GitHub Pages

on:
  push:
    branches:
      - main

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 22
      - name: Install Dependencies
        run: npm ci
      - name: Build Quartz
        run: npm run build
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3
        with:
          path: public
```

## Cloudflare Pages

1. Connect your GitHub repository to Cloudflare Pages
2. Set build command to: `npm run build`
3. Set build output directory to: `public`
4. Deploy!

## Self-Hosting

Copy the contents of the `public` folder to any web server. Quartz works on any static hosting service.

For servers that don't support clean URLs (like Apache), you may need to configure URL rewriting to handle `.html` extensions.
