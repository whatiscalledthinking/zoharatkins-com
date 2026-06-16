# zoharatkins.com

Static Cloudflare-hosted site for `zoharatkins.com`.

## Local preview

```bash
python3 -m http.server 4173
```

Open `http://localhost:4173/`.

## Deploy

This site has no build step. `worker.js` embeds the static pages and image assets and serves them from a Cloudflare Worker attached to both live hostnames.

```bash
bunx wrangler deploy
```

The live routes are:

- `zoharatkins.com`
- `www.zoharatkins.com`

## Notes

- The site intentionally removes Squarespace-generated scripts and CSS.
- Images used on the public site are stored locally in `assets/`.
- The previous Squarespace contact form was replaced with a public-channel contact page because Squarespace form handling cannot be migrated as a static file.
