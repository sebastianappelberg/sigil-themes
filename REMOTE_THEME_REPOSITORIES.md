# Remote Theme Repositories

Sigil can install themes from GitHub repositories. Theme metadata is read from:

- `sigil-themes.json`
- `.sigil/themes.json`

If your repository URL includes `/tree/<ref>/<path>`, Sigil resolves manifests relative to that path.

## Manifest Schema

```json
{
  "schemaVersion": 1,
  "themes": [
    {
      "id": "aurora",
      "name": "Aurora",
      "version": "1.0.0",
      "stylesheet": "themes/aurora.css",
      "description": "Optional description",
      "sourceUrl": "https://example.com/theme-docs"
    }
  ]
}
```

Rules:

- `id` must be unique in the manifest.
- `version` must be `major.minor.patch`.
- `stylesheet` must be a safe relative path (no absolute paths, no `..`).
