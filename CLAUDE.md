# Masks: Villains Pack

Content pack containing villain NPCs from the Masks: A New Generation core rulebook.

## Overview

- **Module ID:** `masks-villains`
- **Type:** Content pack (Actor compendium)
- **Dependency:** Requires `masks-newgeneration-unofficial`
- **Content:** 55 villain NPCs

## Structure

```
masks-villains/
├── module.json           # Module manifest
├── packs/villains/       # LevelDB compendium (gitignored)
├── src/packs/villains/   # JSON source files (version controlled)
├── images/villains/      # NPC portraits
├── tools/                # Pack conversion scripts
└── package.json
```

## Commands

```bash
npm install              # Install dependencies
npm run pullJSONtoLDB    # JSON → LevelDB (after git pull)
npm run pushLDBtoJSON    # LevelDB → JSON (for version control)
```

**Important:** Foundry must be closed when running pack conversion.

## Image Paths

Images are referenced as: `modules/masks-villains/images/villains/{filename}`

## Editing Content

1. Make changes in Foundry
2. Close Foundry (or go to welcome screen)
3. Run `npm run pushLDBtoJSON`
4. Commit the JSON changes

## JSON File Naming

Files follow the pattern: `{type}_{SafeName}_{id}.json`
- Example: `npc_Aquaria_1f936ZKryEmqEqQA.json`
