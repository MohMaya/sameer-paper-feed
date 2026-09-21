# Sameer daily paper RSS

Image-capable RSS for Readwise Reader. Pattern mirrors `shiv-podcast-feeds` (GitHub Pages + unguessable token path).

## Public RSS URL

`https://mohmaya.github.io/sameer-paper-feed/feeds/1VmfXNUkh-XVFhGMbzOlGxKhUBvJu6UA/rss.xml`

Token also in `feed_meta.json`. Do not paste into Slack.

## Layout

- `editions/YYYY-MM-DD/` — markdown edition artifacts
- `feeds/<token>/rss.xml` — **live Pages path** (repo root, same as podcast feeds — not under `public/`)
- `feeds/<token>/store.json` — channel + items for RSS render (also mirrored at `store.json` root)
- `index.html` / `feeds/index.html` — private; no directory listing of tokens

## Status

**GitHub Pages live** from `main` branch path `/`. Public RSS URL above.

## Publish

1. Write edition markdown under `editions/`
2. Append item to `feeds/<token>/store.json` (and/or root `store.json`) — title, link, description/html, optional image, guid, pubDate
3. Render `rss.xml` into `feeds/<token>/` at repo root
4. Commit + push so Pages updates
