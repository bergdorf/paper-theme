# Paper Theme for VS Code

A family of ergonomic, easy-on-the-eyes VS Code color themes built around an ink-on-paper aesthetic. Monochromatic syntax highlighting — weight, not color, creates hierarchy — with comments as the sole accent.

## Variants

| Theme | Type | Background | Character |
|---|---|---|---|
| **Paper Light** | light | `#F6F2ED` | Warm parchment — the base |
| **Paper Soft** | light | `#F6F2ED` | Same as Light, reduced contrast (~5:1) |
| **Paper Warm** | light | `#F2E8D5` | Aged amber, old-book warmth |
| **Paper Cool** | light | `#F0F3F6` | Blue-gray daylight, airy and clean |
| **Paper Dark** | dark | `#1A1714` | True inversion — warm dark, cream text |

## Design principles

- **Monochromatic syntax** — all code tokens use shades of the same warm gray. Color is never used to distinguish syntax categories.
- **Weight as hierarchy** — keywords, type names, function definitions, and other structural elements are **bold**; variables, strings, and operands are normal weight.
- **Comments stand apart** — the one non-monochromatic element. Each variant picks a muted accent that harmonizes with its background without competing with code.
- **Ergonomic contrast** — foreground/background contrast targets ~8:1 (not the harsh 12:1+ of pure black on white). Paper Soft targets ~5:1 for very long sessions.
- **Warm backgrounds** — never pure white. The warmth reduces the blue-light harshness of bright screens.

## Installation

### From VSIX
Download the latest `.vsix` from [Releases](../../releases) and install:
```
code --install-extension paper-theme-*.vsix
```
Or drag the file into the VS Code Extensions panel.

### Manual (clone)
```bash
git clone https://github.com/bergdorf/paper-theme ~/.vscode/extensions/paper-theme
```
Then restart VS Code and select a Paper variant from `Preferences: Color Theme`.

## Selecting a theme

`Ctrl+Shift+P` (or `⌘⇧P`) → `Preferences: Color Theme` → search **Paper**

## Language support

Full token coverage for:
- TypeScript / JavaScript / JSX / TSX
- Python (including docstrings)
- Rust
- Go
- HTML / CSS
- Markdown
- JSON

Semantic highlighting is enabled for TypeScript (tsserver), Python (Pylance), and Rust (rust-analyzer).
