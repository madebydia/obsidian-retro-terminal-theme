# Obsidian Community Theme — Publishing Checklist

Theme: **Retro Terminal**
Date: 2026-02-21

## Requirements (from [obsidian-releases](https://github.com/obsidianmd/obsidian-releases))

### ✅ Done

- [x] **`manifest.json`** — Present with `name`, `version`, `minAppVersion`, `author`, `authorUrl`
- [x] **`theme.css`** — Main stylesheet exists
- [x] **`README.md`** — Includes description, features, installation instructions
- [x] **Supports both dark and light modes** — README documents both; CSS has both
- [x] **Unique theme name** — "Retro Terminal" doesn't appear in community-css-themes.json

### ❌ Still Needed

- [ ] **Screenshot image file** — Must be in the repo root (e.g. `screenshot.png`). Referenced by `screenshot` field in the community-css-themes.json PR. **No screenshot exists yet.**
- [ ] **LICENSE file** — Required for community submissions. Recommended: MIT or GPL. **No LICENSE file exists.**
- [ ] **Dedicated GitHub repository** — Theme needs its own public GitHub repo (e.g. `robutsume/obsidian-retro-terminal-theme`). Currently lives inside the workspace mono-repo, not a standalone repo.
- [ ] **GitHub Release** — Obsidian pulls theme files from the repo's default branch, but having a proper release/tag is good practice.
- [ ] **PR to `community-css-themes.json`** — Add entry to the end of [obsidianmd/obsidian-releases/community-css-themes.json](https://github.com/obsidianmd/obsidian-releases/blob/master/community-css-themes.json):
  ```json
  {
    "name": "Retro Terminal",
    "author": "robutsume",
    "repo": "robutsume/obsidian-retro-terminal-theme",
    "screenshot": "screenshot.png",
    "modes": ["dark", "light"]
  }
  ```
- [ ] **Conform to [Obsidian Developer Policies](https://docs.obsidian.md/Developer+policies)** — Review and confirm compliance

### 💡 Recommended (not strictly required)

- [ ] Add a preview/demo GIF showing both modes
- [ ] Test with popular community plugins (Dataview, Calendar, Kanban, etc.)
- [ ] Test on mobile (iOS/Android)
- [ ] Add Style Settings plugin support for customization
- [ ] Consider adding `publish.css` for Obsidian Publish support

## Steps to Publish

1. Create LICENSE file (MIT recommended)
2. Take a clean screenshot of the theme (dark mode preferred as primary)
3. Push to a dedicated public GitHub repo: `robutsume/obsidian-retro-terminal-theme`
4. Ensure `theme.css` and `manifest.json` are at repo root
5. Fork `obsidianmd/obsidian-releases`
6. Add theme entry to end of `community-css-themes.json`
7. Open PR — use the submission checklist template when creating
8. Wait for review from Obsidian team
