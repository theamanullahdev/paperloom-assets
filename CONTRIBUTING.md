# Contributing

## A look (`widgets/<folder>/`)

- `skin.toml` (format: the app repository's `AGENTS.md`, "Looks / skins", and the built-in looks in `crates/paperloom-skin/skins/`).
- Optional `fonts/` (TTF/OTF, **OFL only**, with the licence file beside the font) and `images/` (PNG).
- The folder name is used in the address; `id` in `skin.toml` is `author/name`.

## A stack (`widgets/stacks/<folder>/`)

`stack.toml`: `id`, `name`, `size = [w, h]` and a `[[widget]]` list (`kind`, `skin`, `dx`, `dy`). Looks it uses that are not built into the app must exist in this repository.

## A theme (`themes/<folder>/`)

`theme.toml` (the `id` must equal the folder name), optional fonts and PNG pictures. In the app: Settings → Appearance → New theme builds one with pickers; Export saves a folder you can copy here.

## Limits and rules

- File types: `.toml`, `.ttf`, `.otf`, `.png`, `.txt`. No scripts, no executables.
- At most 12 MB per item; previews at most 300 KB (they are drawn for you).
- Only things you made or may share. Say who made it (`author`) and keep any licence files.
- Nothing hateful, deceptive or that hides what it does.

The pull request check runs the app's own validator. Warnings stop the build too, so the library stays clean.
