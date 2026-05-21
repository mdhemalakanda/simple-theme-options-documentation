# Simple Theme Options Documentation

Standalone integrator guide for **[Topten Simple Theme Options](https://github.com/hsbeauty39/simple-theme-options)** — how to register menus, sections, fields, read options in themes, and use every field type.

This repository ships **only** the browser documentation (no WordPress plugin code). Use it to onboard theme developers, agencies, and clients who need copy-paste PHP samples and field reference tables.

## View the guide

| How | URL / steps |
|-----|-------------|
| **GitHub Pages (recommended)** | [https://mdhemalakanda.github.io/simple-theme-options-documentation/](https://mdhemalakanda.github.io/simple-theme-options-documentation/) — opens `instructions.html` via `index.html` |
| **Direct file** | Open [`instructions.html`](instructions.html) in this repo on GitHub, or clone and open locally |
| **Local clone** | `git clone …` then open `instructions.html` in Chrome/Firefox/Safari (needs internet for Google Fonts + Prism CDN) |

## What is inside

- **`instructions.html`** — WooCommerce-style three-column guide (nav · prose · PHP snippets), quick search, mobile drawer, live centre ↔ PHP scroll sync, and inline field previews.
- **`index.html`** — redirect to the guide (GitHub Pages root).

No extra CSS/JS assets are required: layout, scripts, and preview templates are embedded in `instructions.html`.

## Plugin source

Install and develop against the plugin repository:

- **GitHub:** [hsbeauty39/simple-theme-options](https://github.com/hsbeauty39/simple-theme-options)
- **Folder name:** use `topten-simple-theme-options` or `battery-simple-theme-options` in `wp-content/plugins/` — **not** the wordpress.org slug `simple-theme-options` (different plugin).

The canonical HTML for this docs repo is maintained in the plugin workspace at `wp-content/plugins/instructions/instructions.html`. When field types or admin UX change, update that file in the plugin project, then copy the refreshed `instructions.html` here.

## Maintenance (plugin workspace)

From `wp-content/plugins/instructions/` in a full WordPress dev site:

```bash
python3 scripts/generate-field-docs.py
python3 scripts/inject-php-snippet-theme-usage.py
python3 scripts/reformat-instructions-prose.py
```

Then copy `instructions.html` into this repository and commit.

## License

Documentation follows the same licensing terms as the Topten Simple Theme Options plugin you distribute. Do not republish the plugin ZIP inside this repo.
