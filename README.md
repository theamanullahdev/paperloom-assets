# Paperloom assets

The online library that [Paperloom](https://github.com/theamanullahdev/paperloom) reads from: **widget looks**, **stacks of widgets** and **app themes**. Paperloom's Browse → Online pages, the website's [library page](https://theamanullahdev.github.io/paperloom/library.html) and the MCP tools all read the `index.json` files in this repository.

```
widgets/            looks (one folder each, with skin.toml) and widgets/stacks/ (stack.toml)
themes/             app themes (one folder each, with theme.toml)
scripts/            build-widgets-index.py, build-themes-index.py
```

Every folder has a `preview.png`. `index.json` lists each file with its SHA-256 and size; Paperloom installs an item only if every file matches. **Don't edit `index.json` or `preview.png` by hand**: automation rebuilds both on every push.

## Adding something

1. Fork this repository and add a folder under `widgets/`, `widgets/stacks/` or `themes/`. See [CONTRIBUTING.md](CONTRIBUTING.md) for what a folder holds and the limits.
2. Open a pull request. A check runs the same validation the app uses and tells you what to fix.
3. When it is merged, the library updates itself and the item appears in the app and on the website within minutes.

(A "Submit to the library" button in the app is planned.)

## Licences

Each item belongs to its author and carries the licence it was shared under (fonts must be OFL and ship their licence file next to them). Items by "Paperloom" are GPL-3.0-or-later, like the app. See [NOTICE](NOTICE).
