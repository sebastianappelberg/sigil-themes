# sigil-themes

Theme pack repository for Sigil.

## Included themes

- `rainbow` (`themes/rainbow.css`): bright, playful palette with rainbow accent gradients.
- `hacker` (`themes/hacker.css`): dark terminal-inspired palette with neon green accents.
- `intellij-dark` (`themes/intellij-dark.css`): IntelliJ-inspired graphite dark palette with cool blue focus and warm accents.

## Manifest

Sigil reads available themes from [`sigil-themes.json`](./sigil-themes.json):

- `schemaVersion`: manifest schema version.
- `themes[].id`: unique theme identifier.
- `themes[].name`: display name in Sigil.
- `themes[].version`: semantic version (`major.minor.patch`).
- `themes[].stylesheet`: relative path to the CSS file.
- `themes[].description`: optional theme description.

## Using this repository in Sigil

1. Copy the repository URL.
2. Add it as a remote theme repository in Sigil.
3. Sigil will load `sigil-themes.json` and make listed themes available.

For manifest path and compatibility details, see [`REMOTE_THEME_REPOSITORIES.md`](./REMOTE_THEME_REPOSITORIES.md).
