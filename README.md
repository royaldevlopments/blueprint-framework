# Royal Blueprint 🚀

**Blueprint Framework fork** — specially built for **Royal Panel** by **Shaurya Vashishtha (Royal Devlopments)**.

## What is this?

A fully Arix Theme-compatible version of Blueprint Framework. Install extensions on your Pterodactyl/Royal Panel without breaking your Arix theme.

## Features

- ✅ **Arix Theme auto-detection** — detects Arix during install
- ✅ **Zero manual merging** — restores Arix React components, templates, and config automatically
- ✅ **Blueprint directives auto-merged** — all `@include`/`@yield` directives added to Arix templates
- ✅ **All Blueprint extensions work** — install/uninstall extensions normally
- ✅ **No branding conflicts** — clean integration with Royal Panel

## Installation

```bash
# Extract release over your panel root
unzip release.zip -d /var/www/pterodactyl

# Run installer
bash blueprint.sh
```

The installer automatically handles Arix compatibility. No manual file merging needed.

## Requirements

- Pterodactyl/Royal Panel with Arix Theme v2.x installed
- PHP 8.0+, Node 22+, MariaDB/MySQL

## Maintainer

**Shaurya Vashishtha** — Royal Devlopments

---

*Based on Blueprint Framework — modified for Royal Panel compatibility*
