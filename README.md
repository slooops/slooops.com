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

- Cloudflare caps each file at 25 MB. Compress big PDFs first:
  `gs -sDEVICE=pdfwrite -dPDFSETTINGS=/printer -dColorConversionStrategy=/RGB -dColorImageResolution=220 -dGrayImageResolution=220 -dNOPAUSE -dBATCH -sOutputFile=out.pdf in.pdf`
- Derived from [slooops.github.io](https://github.com/slooops/slooops.github.io), minus the code-stats chart.
