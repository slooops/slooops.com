# Jack Sloop • slooops.com

Personal portfolio, plus privacy policies and App Store links for my iOS apps.

## Stack

- Plain HTML/CSS, no build step — everything served lives in `public/`
- Inter / Inter Display via rsms.me
- Hosted on Cloudflare Workers (static assets), config in `wrangler.jsonc`

## Develop & deploy

```bash
npx wrangler dev      # local preview at http://localhost:8787
npx wrangler deploy   # ship to slooops.com
```

## Notes

- `Reunion.pdf` (51 MB) is over Cloudflare's 25 MB per-file asset limit, so the archive links to the copy on slooops.github.io.
- Derived from [slooops.github.io](https://github.com/slooops/slooops.github.io), minus the code-stats chart.
