# Stardust Liar Transformation Summary

This document summarizes the transformation of the Stardust-Liar repository from an empty repository to a complete Jekyll campaign homepage.

## Source Material

The structure and approach were inspired by the JakeAO/Vaultlight repository, a noir heist campaign hub. However, all content has been completely reimagined for the Stardust Liar setting.

## Setting: Stardust Liar

**Genre:** Gritty sci-fi (Star Wars meets Cowboy Bebop)

**Tone:** Cynical but hopeful—"the trash bin of space"

**Core Themes:**
- Survival in a hostile, uncaring galaxy
- Corrupt planetary governments and syndicate control
- Volunteer aide organizations struggling to help
- Rare pockets of community and mutual aid
- People trying to do right despite overwhelming odds

## Visual Design

**Color Palette:**
- Muted, industrial tones
- Rusted bronze (#8a6f47) for primary accents
- Oxidized green (#5a6b5e) for secondary elements
- Faded grey (#d4d4d4) for text
- Deep void black (#0d0d0d) for backgrounds

**Typography:**
- Headers: Impact, Franklin Gothic Bold (hard-edged, industrial)
- Body: Consolas, Monaco, Courier New (utilitarian monospace)
- All uppercase headers with heavy weight

**Visual Elements:**
- Layered panel aesthetics
- Rivets and seams suggesting worn infrastructure
- Muted texture overlays
- Minimal decoration—everything serves function

## Content Created

### Core Pages
- `index.md` - Homepage introducing the setting and premise
- `world.md` - Galaxy information landing page
- `info.md` - FATE Condensed rules reference
- `sessions.md` - Session logs landing page
- `gm-notes.md` - Private GM content access

### Example Factions (3)
1. **Harkan Syndicate** - Criminal organization controlling Sector 7
2. **Makara Planetary Authority** - Corporate-controlled planetary government
3. **Horizon Aid Collective** - Volunteer humanitarian fleet

### Example Locations (2)
1. **Harkan Station** - Syndicate-controlled trade hub
2. **Rust Haven Station** - Independent community-run station

### Example NPCs (3)
1. **Kella Harkan** - Ruthless syndicate boss
2. **Dr. Amara Chen** - Stubborn humanitarian doctor
3. **Jaxx "Wrench" Kovar** - Independent mechanic and smuggler

### Documentation
- FATE mechanics explanation (aspects)
- Templates for creating NPCs, factions, locations, sessions
- Comprehensive README with setup instructions

## Technical Implementation

**Framework:** Jekyll 4.x with GitHub Pages

**Theme:** Minima (heavily customized)

**Collections:**
- `_info` - Rules and mechanics
- `_world` - Setting, characters, factions, locations
- `_sessions` - Session summaries
- `_gm` - Private GM content

**Deployment:** Automated via GitHub Actions

## Key Design Decisions

1. **Simplified styling**: Created a streamlined SCSS file focusing on the core aesthetic rather than extensive visual effects
2. **Content-first approach**: Prioritized creating rich, evocative world content over technical features
3. **Tone consistency**: Every piece of content reinforces the "cynical but hopeful" survival theme
4. **Practical templates**: Simple, clear templates for adding new content
5. **Clear navigation**: Three main sections (Info, Galaxy, Sessions) with consistent structure

## Future Extensions

The structure supports easy expansion:
- Additional factions representing different power structures
- More locations in various sectors
- Character roster as campaigns progress
- Session summaries documenting gameplay
- GM content for secrets and planning

## Acknowledgments

- Structure inspired by JakeAO/Vaultlight
- Built with Jekyll and Minima theme
- Powered by FATE Condensed RPG system
- Deployed via GitHub Pages
