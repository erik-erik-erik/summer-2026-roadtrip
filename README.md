# Summer 2026 Roadtrip

A working plan for a 9-week northern loop from Park City, UT to Lopez Island, WA and back, by truck camper.

**Live page:** https://erik-erik-erik.github.io/summer-2026-roadtrip/ *(once published)*

## What's in here

- `index.html` — single self-contained page with route map, destination previews, tradeoff discussion, and full itinerary index. Open it directly in any browser.

## Publishing to GitHub Pages

One-time setup, from this directory:

```bash
git init -b main
git add .
git commit -m "Initial commit"
gh repo create summer-2026-roadtrip --public --source=. --push
gh repo edit --enable-pages --pages-source main
```

If you don't have the GitHub CLI (`gh`) installed:

```bash
# Manual path: create the repo on github.com first, then:
git init -b main
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:erik-erik-erik/summer-2026-roadtrip.git
git push -u origin main
# Then in repo Settings → Pages → set source to "main" branch / root
```

Pages takes 1–2 minutes to build. The URL will be:

```
https://erik-erik-erik.github.io/summer-2026-roadtrip/
```

## Updating

Edit `index.html`, then:

```bash
git add index.html && git commit -m "Update" && git push
```

Pages will rebuild automatically.
