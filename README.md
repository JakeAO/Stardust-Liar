# Stardust Liar Campaign Hub

A Jekyll-based static site for the Stardust Liar TTRPG campaign, featuring a gritty, rundown, dystopian aesthetic.

## Overview

This repository hosts the campaign hub for **Stardust Liar**, a narrative campaign set in a dying world where infrastructure crumbles, lights flicker, and survival is the only goal that matters.

## Features

- **Public Player Content:**
  - Rules & Info: Game mechanics and reference materials
  - World: Setting, characters, locations, and factions
  - Sessions: Chronological session summaries
  
- **Private GM Content:**
  - Accessible via obscured URL (`/gm-vault-7d4b2e/`)
  - Campaign planning and session prep
  - Hidden character motivations
  - World secrets and plot threads
  - Not indexed by search engines (via robots.txt)

- **Theme:**
  - Gritty, rundown aesthetic with rusted metal and failing infrastructure
  - Dark dystopian atmosphere with flickering amber lights
  - Weathered typography and decaying visuals
  - Mobile-responsive design

## Local Development

### Prerequisites

- Ruby 3.1 or higher
- Bundler gem

### Setup

```bash
# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

The site will be available at `http://localhost:4000`

## Project Structure

```
.
├── _config.yml           # Jekyll configuration
├── _info/                # Rules and mechanics (public)
├── _world/               # Campaign world content (public)
│   ├── npcs/             # Non-player characters
│   ├── locations/        # Places in the world
│   └── factions/         # Organizations and groups
├── _sessions/            # Session summaries (public)
├── _gm/                  # GM-only content (private URL)
├── _templates/           # Content templates
├── assets/css/           # Custom styling
├── index.md              # Home page
├── info.md               # Rules landing page
├── world.md              # World landing page
├── sessions.md           # Sessions landing page
└── gm-notes.md           # GM vault landing page
```

## Adding Content

### Public Content

Create new markdown files in the appropriate collection folder using the templates in `_templates/`:

**NPC Example:**
```markdown
---
layout: page
title: Character Name
topic: NPCs
summary: Brief description
---

# Character Name

Full content here...
```

**Session Example:**
```markdown
---
layout: page
title: Session Title
index: 1
summary: Brief summary
---

# Session 1: Title

Full session summary...
```

### GM Content

Same structure, but place files in `_gm/` directory. These will be published at the obscured URL but won't appear in navigation or search engine indexes.

## Deployment

The site automatically deploys to GitHub Pages via GitHub Actions when changes are pushed to the `main` branch.

### GitHub Pages Setup

1. Go to repository Settings → Pages
2. Set Source to "GitHub Actions"
3. The workflow in `.github/workflows/pages.yml` handles the rest

## Theme Customization

The site uses Jekyll's Minima theme with extensive customization in `assets/css/style.scss`. The color scheme features:

- Rusted orange and tarnished gold accents
- Brown-tinged dark backgrounds (rust, dirt, decay)
- Flickering amber highlights (failing lights)
- Weathered, gritty textures

## Contributing

This is a private campaign repository. If you're a player, please don't peek at the `_gm/` folder—spoilers ahead!

## License

Campaign content is private. The Jekyll structure and theme are based on open-source components.

## Credits

- Built with [Jekyll](https://jekyllrb.com/)
- Theme based on [Minima](https://github.com/jekyll/minima)
- Structure inspired by [Vaultlight](https://github.com/JakeAO/Vaultlight)
