# Theming Contract

## Required `theme.css` Sections

Keep this section structure in `theme.css`:

1. `/* Theme Metadata */`
2. `/* Token Overrides */`
3. `/* Component Overrides (optional) */`
4. `/* Accessibility Guardrails */`

## Token Reference

Define tokens in `:root { ... }`.

### Typography

- `--ds-font-family`
- `--ds-font-size-base`
- `--ds-font-size-sm`
- `--ds-font-size-lg`
- `--ds-font-weight-normal`
- `--ds-font-weight-medium`
- `--ds-font-weight-semibold`
- `--ds-line-height-base`

### Colors

- `--ds-color-bg`
- `--ds-color-surface`
- `--ds-color-surface-alt`
- `--ds-color-surface-elevated`
- `--ds-color-text`
- `--ds-color-text-muted`
- `--ds-color-border`
- `--ds-color-accent`
- `--ds-color-accent-contrast`
- `--ds-color-success`
- `--ds-color-warning`
- `--ds-color-danger`
- `--ds-color-focus`

### Shape and depth

- `--ds-radius-sm`
- `--ds-radius-md`
- `--ds-radius-lg`
- `--ds-radius-xl`
- `--ds-border-width`
- `--ds-shadow-sm`
- `--ds-shadow-md`
- `--ds-shadow-lg`
- `--ds-overlay-blur`

### State

- `--ds-state-hover-bg`
- `--ds-state-selected-bg`
- `--ds-state-active-bg`
- `--ds-state-disabled-opacity`
- `--ds-state-focus-ring`

### Density and spacing

- `--ds-control-height-sm`
- `--ds-control-height-md`
- `--ds-control-padding-x`
- `--ds-control-padding-y`
- `--ds-list-item-padding-x`
- `--ds-list-item-padding-y`
- `--ds-gap-sm`
- `--ds-gap-md`

### Motion

- `--ds-motion-enabled`
- `--ds-duration-fast`
- `--ds-duration-normal`
- `--ds-ease-standard`

### Scrollbar and icons

- `--ds-scrollbar-size`
- `--ds-scrollbar-track`
- `--ds-scrollbar-thumb`
- `--ds-scrollbar-thumb-hover`
- `--ds-icon-size-sm`
- `--ds-icon-size-md`
- `--ds-icon-opacity-muted`

## Stable Selectors and Attributes

### Modes

- `.ds-root`
- `[data-mode="provider_picker"]`
- `[data-mode="query"]`
- `[data-mode="settings"]`

### Layout

- `.ds-overlay`
- `.ds-header`
- `.ds-search`
- `.ds-results`
- `.ds-panel`
- `.ds-card`

### Controls

- `.ds-input-shell`
- `.ds-input`
- `.ds-select`
- `.ds-checkbox`
- `.ds-button[data-variant]`
- `.ds-badge[data-variant]`

### Lists

- `.ds-list`
- `.ds-list-item`
- `.ds-list-title`
- `.ds-list-description`
- `.ds-list-empty`
- `.ds-list-skeleton`

### State hooks

- `[data-selected="true"]`
- `[data-disabled="true"]`
- `[data-voice-state="idle"]`
- `[data-voice-state="listening"]`
- `[data-voice-state="unavailable"]`
