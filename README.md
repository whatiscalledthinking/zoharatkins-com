# zoharatkins.com

Static Cloudflare Pages site for `zoharatkins.com`.

## Local preview

```bash
python3 -m http.server 4173
```

Open `http://localhost:4173/`.

## Deploy

This site has no build step. Deploy the repository root to Cloudflare Pages.

```bash
bunx wrangler pages deploy . --project-name zoharatkins-com
```

The live custom domains should be:

- `zoharatkins.com`
- `www.zoharatkins.com`

## Notes

- The site intentionally removes Squarespace-generated scripts and CSS.
- Images used on the public site are stored locally in `assets/`.
- The previous Squarespace contact form was replaced with a public-channel contact page because Squarespace form handling cannot be migrated as a static file.
