# Stardust Liar Campaign Hub

A Jekyll-based static site for the Stardust Liar TTRPG campaign, featuring a gritty sci-fi aesthetic inspired by Star Wars and Cowboy Bebop.

## Overview

This repository hosts the campaign hub for **Stardust Liar**, a FATE Condensed campaign set in the corrupt, patchwork remains of a galactic civilization. Players navigate syndicate-controlled sectors, corrupt planetary governments, and volunteer aide networks while trying to survive in "the trash bin of space."

## Features

- **Public Player Content:**
  - Rules & Info: FATE Condensed mechanics and cheat sheets
  - Galaxy: Setting, revealed NPCs, locations, and factions
  - Session Logs: Chronological session summaries
  
- **Private GM Content:**
  - Accessible via obscured URL (`/gm-vault-32f8a9/`)
  - Campaign planning and arc notes
  - Hidden NPCs and secret motivations
  - World secrets and faction agendas
  - Not indexed by search engines (via robots.txt)

- **Theme:**
  - Gritty, grimy, industrial aesthetic
  - Muted color palette (rusted metals, oxidized greens, faded greys)
  - Hard-edged typography with utilitarian feel
  - Layered, rundown visual design
  - Mobile-responsive layout

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
│   ├── mechanics/        # FATE mechanics explanations
│   └── cheat-sheets/     # Quick reference sheets
├── _world/               # Campaign world content (public)
│   ├── npcs/             # Non-player characters
│   ├── locations/        # Stations, planets, sectors
│   └── factions/         # Syndicates, governments, groups
├── _sessions/            # Session summaries (public)
├── _gm/                  # GM-only content (private URL)
│   ├── planning/         # Campaign and session planning
│   ├── npcs/             # Secret NPC information
│   └── secrets/          # Hidden world lore
├── assets/css/           # Custom styling
├── index.md              # Home page
├── info.md               # Rules landing page
├── world.md              # Galaxy landing page
├── sessions.md           # Sessions landing page
└── gm-notes.md           # GM vault landing page
```

## Adding Content

### Public Content

Create new markdown files in the appropriate collection folder:

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

**Faction Example:**
```markdown
---
layout: page
title: Faction Name
topic: Factions
summary: Brief description
---

# Faction Name

Full faction information...
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

The site automatically deploys to GitHub Pages via GitHub Actions when changes are pushed to the `main` or `master` branch.

### GitHub Pages Setup

1. Go to repository Settings → Pages
2. Set Source to "GitHub Actions"
3. The workflow in `.github/workflows/pages.yml` handles the rest

## Theme Customization

The site uses Jekyll's Minima theme with extensive customization in `assets/css/style.scss`. The gritty sci-fi aesthetic features:
- Muted, industrial color palette
- Hard-edged, uppercase typography
- Layered visual elements suggesting worn panels
- Subtle texture overlays for a rundown feel

## Setting

**Stardust Liar** is set in a galaxy where:
- The Galactic Coalition has collapsed
- Planetary governments are corrupt and syndicate-controlled
- Volunteer aide fleets struggle to help forgotten communities
- Survival means navigating a hostile, uncaring universe
- Hope exists in small acts of kindness and solidarity

The tone is cynical but hopeful—"the trash bin of space" where people keep going despite everything.

## Contributing

This is a private campaign repository. If you're a player, please don't peek at the `_gm/` folder—spoilers ahead!

## License

Campaign content is private. The Jekyll structure and theme are based on open-source components.

## Credits

- Built with [Jekyll](https://jekyllrb.com/)
- Theme based on [Minima](https://github.com/jekyll/minima)
- Powered by [FATE Condensed](https://www.evilhat.com/home/fate-condensed/)
- Structure inspired by Vaultlight campaign hub
