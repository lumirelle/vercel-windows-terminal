# Vercel for Windows Terminal

Two variants: dark and light.

## Sources

- Colors: [gantoreno/vscode-vercel `themes`](https://github.com/gantoreno/vscode-vercel/tree/main/themes)

## Mapping

| Key | Dark | Light |
|-----|------|-------|
| background | `#000000` | `#FFFFFF` |
| foreground | `#EDEDED` | `#171717` |
| cursorColor | foreground | foreground |
| selectionBackground | `#333333` | `#CCCCCC` |
| black | ansiBlack | ansiBlack |
| white | ansiWhite | ansiWhite |
| purple | ansiMagenta | ansiMagenta |
| tab.background | `#0A0A0A` | `#FFFFFF` |
| tabRow.background | `#000000` | `#FAFAFA` |

## Usage

Copy the variant you want:

1. Copy the raw content of `variant.jsonc` into `schemes` field of Windows Terminal's configuration file `settings.json`;
2. Copy the raw content of `variantTheme.jsonc` into `themes` field of Windows Terminal's configuration file `settings.json`;
3. Choose the scheme and theme in Windows Terminal's settings;
4. Enjoy!
