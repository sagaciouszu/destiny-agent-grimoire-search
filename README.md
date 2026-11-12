# Destiny Agent Grimoire — Search Edition

This repository is a fork of
[destiny-agent-grimoire-site](https://github.com/sagaciouszu/destiny-agent-grimoire-site)
with full-text search added via [Pagefind](https://pagefind.app/).

## What's different

- `npm run build` runs Eleventy then Pagefind, producing a searchable `_site/`.
- `/search/` page with the Pagefind UI.
- Search link in the primary navigation.
- Search covers site documentation (guides, install, troubleshooting, persona
  pages, limits). It does **not** search the 125,324 lore lines in the Grimoire
  database — that requires a local install (see the install guide).

## Build

```bash
npm install
npm run build
npx serve _site
```

## Search locally

After building, open `_site/search/index.html` in a browser, or serve `_site/`
and visit `/search/`.

## Relationship to the main site

This repo tracks the main site and adds search. To sync upstream changes:

```bash
git remote add upstream https://github.com/sagaciouszu/destiny-agent-grimoire-site.git
git fetch upstream
git merge upstream/main
```
