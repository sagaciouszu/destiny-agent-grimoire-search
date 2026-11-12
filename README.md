# Destiny Agent Grimoire — Search (archived)

> **Archived.** Search now ships in the main site:
> <https://sagaciouszu.github.io/destiny-agent-grimoire-site/search/>

This repository was the Pagefind prototype. The integration was folded into
[destiny-agent-grimoire-site](https://github.com/sagaciouszu/destiny-agent-grimoire-site)
so the project keeps one deploy, one stats snapshot and no drift between a fork
and its upstream.

The `backup/pre-search` branch holds the pre-search baseline of the site.

## What moved

- `npm run build` in the main site runs Eleventy then Pagefind.
- `/search/` uses the Pagefind Component UI with `bundle-path` and `base-url`
  set to the Pages subpath.
- Search covers site documentation only. Lore search stays local in the
  Grimoire CLI and MCP server.

Nothing here is maintained. Use the main site repository.
