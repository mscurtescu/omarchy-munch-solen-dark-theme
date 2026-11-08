# Changelog — Munch Solen Dark

Follows the theme payload in this repo; released by pushing to `master`.

## [Unreleased]

- Drop `hyprland.lua` from the theme, including the `.example` reference.
  Omarchy regenerates the Hyprland config from `colors.toml`, which still
  paints the 3-stop ray gradient. A listed theme may not ship scripts.
- Stop tracking the Beads git hooks under `.beads/hooks/`. They are local
  authoring tools, not part of the theme.
- Stop tracking `.claude/settings.json` and `.codex/hooks.json`. They are
  local Claude Code and Codex hook configs. `bd setup claude` and
  `bd setup codex` rewrite them.
- Re-encode the three backgrounds as WebP (`-strip -resize '3840>' -quality 82`):
  the set drops from 6.6 MB to 3.7 MB, with `1-solen` alone going 4.5 MB → 2.4 MB.

## [1.0.0] - 2026-09-14

First gallery-ready release.

- Three wallpapers: full mural plus sun-disk and ray detail crops.
- Desktop-screenshot `preview.webp`; empty-desktop shots (`wallpaper.webp`,
  `wallpaper-disk.webp`, `wallpaper-rays.webp`) in the README.
- `DESIGN.md` design notes; trimmed README with palette table, sibling
  and Island Bar cross-links, and badges.

## [0.1.0] - 2026-09-11

Initial public release.

- Indigo rock-cleft surfaces, cadmium-ray accent, straw-halo type.
- Animated 3-stop solar window border (`hyprland.lua`, symlink installs).
- Full hand-written `shell.toml` chrome.
- Single Aula-mural wallpaper (`backgrounds/1-solen.jpg`, UiO CC BY-NC-SA).
