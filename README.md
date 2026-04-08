# Astrio Documentation

This is a documentation for Astrio: doc.astrio.app

## Run locally

1. Install [Node.js](https://nodejs.org/) 18 or newer.
2. From this repository’s root directory:

   ```bash
   npx mintlify dev
   ```

3. Open [http://localhost:3000](http://localhost:3000).

If you prefer a global CLI: `npm install -g mintlify`, then `mintlify dev`.

## Edit content

- **Pages:** `.mdx` files under `introduction/`, `features/`, `integrations/`, `best-practices/`.
- **Nav / theme / tabs:** `mint.json`.
- **Static assets:** `assets/`.

## Deploy

Pushes to `main` run GitHub Actions (link check and deploy to GitHub Pages). Repository settings → Pages → source “GitHub Actions” if you need to enable it.
