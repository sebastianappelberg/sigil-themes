# Theming Contract

Sigil applies one active stylesheet at runtime. The active file can be:

- Local theme: `themes/local/default.css`
- Repository theme: `themes/<repository-id>/<theme-file>.css`

These files are resolved under Sigil app data and hot-reloaded when saved.

## Required Sections

1. `/* Theme Metadata */`
2. `/* Token Overrides */`
3. `/* Component Overrides (optional) */`
4. `/* Accessibility Guardrails */`

## Public Tokens (`--sigil-*`)

Typography:
`--sigil-font-family`, `--sigil-font-size-base`, `--sigil-font-size-sm`, `--sigil-font-size-lg`, `--sigil-font-weight-normal`, `--sigil-font-weight-medium`, `--sigil-font-weight-semibold`, `--sigil-line-height-base`

Colors:
`--sigil-color-bg`, `--sigil-color-surface`, `--sigil-color-surface-alt`, `--sigil-color-surface-elevated`, `--sigil-color-text`, `--sigil-color-text-muted`, `--sigil-color-border`, `--sigil-color-accent`, `--sigil-color-accent-contrast`, `--sigil-color-success`, `--sigil-color-warning`, `--sigil-color-danger`, `--sigil-color-focus`

Shape/depth:
`--sigil-radius-sm`, `--sigil-radius-md`, `--sigil-radius-lg`, `--sigil-radius-xl`, `--sigil-border-width`, `--sigil-shadow-sm`, `--sigil-shadow-md`, `--sigil-shadow-lg`, `--sigil-overlay-blur`

State:
`--sigil-state-hover-bg`, `--sigil-state-selected-bg`, `--sigil-state-active-bg`, `--sigil-state-disabled-opacity`, `--sigil-state-focus-ring`

Density/spacing:
`--sigil-control-height-sm`, `--sigil-control-height-md`, `--sigil-control-padding-x`, `--sigil-control-padding-y`, `--sigil-list-item-padding-x`, `--sigil-list-item-padding-y`, `--sigil-gap-sm`, `--sigil-gap-md`

Motion:
`--sigil-duration-fast`, `--sigil-duration-normal`, `--sigil-ease-standard`

Scrollbar/icons:
`--sigil-scrollbar-size`, `--sigil-scrollbar-track`, `--sigil-scrollbar-thumb`, `--sigil-scrollbar-thumb-hover`, `--sigil-icon-size-sm`, `--sigil-icon-size-md`, `--sigil-icon-opacity-muted`

## Public Selectors (`.sigil-*`)

`.sigil-root`, `.sigil-overlay`, `.sigil-header`, `.sigil-search`, `.sigil-results`, `.sigil-panel`, `.sigil-card`, `.sigil-input-shell`, `.sigil-input`, `.sigil-select`, `.sigil-checkbox`, `.sigil-button[data-variant]`, `.sigil-badge[data-variant]`, `.sigil-list`, `.sigil-list-item`, `.sigil-list-title`, `.sigil-list-description`, `.sigil-list-empty`, `.sigil-list-skeleton`

States and mode hooks:
`data-mode`, `data-selected`, `data-disabled`, `data-voice-state`, `data-variant`

Variants:
- Buttons: `primary`, `secondary`, `ghost`
- Badges: `private`, `custom`, `repository`, `provider-type`
