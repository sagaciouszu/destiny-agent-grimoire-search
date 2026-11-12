---
layout: page
title: Search
category: Search
lede: Search the site — guides, install steps, troubleshooting, persona pages and the limits page.
section: search
---

<figure class="page-hero">
  <img src="{{ '/assets/zero-hour.jpg' | url }}" alt="A red-lit corridor aboard the Almighty." width="1280" height="720" decoding="async">
</figure>

<div id="search"></div>

<link href="{{ '/pagefind/pagefind-ui.css' | url }}" rel="stylesheet">
<script src="{{ '/pagefind/pagefind-ui.js' | url }}" defer></script>
<script>
  window.addEventListener('DOMContentLoaded', () => {
    new PagefindUI({
      element: '#search',
      showSubResults: true,
      showImages: false,
      excerptLength: 20,
    });
  });
</script>

## What you can search here

This search covers the **site documentation** — install guides, troubleshooting,
persona pages, limits and provenance, and the build notes. It does **not** search
the 125,324 lore lines in the Grimoire database.

For lore search, install the Grimoire locally and use the command line:

```bash
python3 db/query.py search "your term" --limit 10
```

Or connect an AI through the MCP server — see
[Connect an AI]({{ '/grimoire/mcp/' | url }}).

## Tips

- Use exact phrases in quotes: `"absolutely not"`.
- Filter by the page you want: type `install` to find setup steps.
- The search is local — nothing is sent anywhere.
