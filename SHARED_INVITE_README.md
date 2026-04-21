# bgulac.github.io - Namaz Vakti Website Files

Upload contents to bgulac.github.io repository.

## Structure
- `h/index.html` — Hatim invite landing (matches `https://bgulac.github.io/h/?c=XXX`)
- `z/index.html` — Zikir group invite landing (matches `/z/?c=XXX`)
- `.well-known/assetlinks.json` — Android App Links verification
- `.well-known/apple-app-site-association` — iOS Universal Links verification (NO file extension!)

## Deployment
1. Copy all files to your bgulac.github.io repo root
2. Commit + push
3. Verify at:
   - https://bgulac.github.io/h/?c=TEST123
   - https://bgulac.github.io/z/?c=TEST456
   - https://bgulac.github.io/.well-known/assetlinks.json
   - https://bgulac.github.io/.well-known/apple-app-site-association

## Notes
- GitHub Pages may not serve `apple-app-site-association` with `Content-Type: application/json` by default. If iOS Universal Links fail, use a `_config.yml` trick or move to Cloudflare Pages.
- Replace App Store ID placeholder (`idXXXXXXXX`) in both HTML files with actual App Store app ID after app is published.
