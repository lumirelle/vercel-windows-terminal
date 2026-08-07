# Vercel Theme for Windows Terminal

Two variants: dark and light.

## Sources

- Colors: [gantoreno/vscode-vercel `themes`](https://github.com/gantoreno/vscode-vercel/tree/main/themes)

## Mapping

Colors are taken from the latest upstream Vercel design tokens
([`TOKENS.md`](https://github.com/lumirelle/vscode-vercel/blob/main/TOKENS.md)).

| Key | Dark | Light |
|-----|------|-------|
| background | `#000000` | `#FFFFFF` |
| foreground | `#EDEDED` | `#171717` |
| cursorColor | `#EDEDED` | `#171717` |
| selectionBackground | `#1A1A1A` | `#F2F2F2` |
| black | `#EDEDED` | `#171717` |
| red | `#C62128` | `#C62128` |
| green | `#00CA50` | `#107D32` |
| yellow | `#FF9300` | `#AA4D00` |
| blue | `#47A8FF` | `#005FF2` |
| purple | `#C472FB` | `#7D00CC` |
| cyan | `#01F7F7` | `#01F7F7` |
| white | `#1A1A1A` | `#F2F2F2` |
| tab.background | `#00000000` | `#FFFFFFFF` |
| tabRow.background | `#000000FF` | `#FFFFFFFF` |
| tabRow.unfocusedBackground | `#000000FF` | `#FFFFFFFF` |

## Usage

Copy the variant you want:

1. Copy the raw content of `variant.jsonc` into `schemes` field of Windows Terminal's configuration file `settings.json`;
2. Copy the raw content of `variantTheme.jsonc` into `themes` field of Windows Terminal's configuration file `settings.json`;
3. Choose the scheme and theme in Windows Terminal's settings;
4. Enjoy!
