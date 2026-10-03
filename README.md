# Vercel Theme for Windows Terminal

Two variants: dark and light.

## Sources

- Colors: [vercel.nvim](https://github.com/lumirelle/vercel.nvim) —
  [`SCHEMA.md`](https://github.com/lumirelle/vercel.nvim/blob/main/SCHEMA.md) /
  [`lua/vercel/colors.lua`](https://github.com/lumirelle/vercel.nvim/blob/main/lua/vercel/colors.lua)

## Mapping

Each value is written as its vercel.nvim palette entry, `scale[step]`, followed by the hex.

| Key | Dark | Light |
|-----|------|-------|
| background | `background[200]` `#000000` | `background[200]` `#FAFAFA` |
| foreground | `gray[1000]` `#EDEDED` | `gray[1000]` `#171717` |
| cursorColor | `gray[1000]` `#EDEDED` | `gray[1000]` `#171717` |
| selectionBackground | `gray[200]` `#1F1F1F` | `gray[200]` `#EBEBEB` |
| black | `gray[1000]` `#EDEDED` | `gray[1000]` `#171717` |
| red | `red[900]` `#FF6166` | `red[900]` `#CB2A2F` |
| green | `green[900]` `#62C073` | `green[900]` `#297A3A` |
| yellow | `amber[900]` `#F2A20D` | `amber[900]` `#A35200` |
| blue | `blue[900]` `#52A8FF` | `blue[900]` `#0068D6` |
| purple | `purple[900]` `#BF7AF0` | `purple[900]` `#7820BC` |
| cyan | `teal[900]` `#0AC7B4` | `teal[900]` `#067A6E` |
| white | `background[100]` `#0A0A0A` | `background[100]` `#FFFFFF` |
| tab.background | transparent `#00000000` | `background[200]` `#FAFAFAFF` |
| tabRow.background | `background[200]` `#000000FF` | `background[200]` `#FAFAFAFF` |
| tabRow.unfocusedBackground | `background[200]` `#000000FF` | `background[200]` `#FAFAFAFF` |

## Usage

Copy the variant you want:

1. Copy the raw content of `variant.jsonc` into `schemes` field of Windows Terminal's configuration file `settings.json`;
2. Copy the raw content of `variantTheme.jsonc` into `themes` field of Windows Terminal's configuration file `settings.json`;
3. Choose the scheme and theme in Windows Terminal's settings;
4. Enjoy!
