# Vercel Theme for Windows Terminal

Two variants: dark and light.

## Sources

- Design system: [Vercel Geist design system](https://vercel.com/geist/introduction)
- Colors: [vercel.nvim](https://github.com/lumirelle/vercel.nvim) —
  [`SCHEMA.md`](https://github.com/lumirelle/vercel.nvim/blob/main/SCHEMA.md) /
  [`lua/vercel/colors.lua`](https://github.com/lumirelle/vercel.nvim/blob/main/lua/vercel/colors.lua)

## Mapping

Every value is a vercel.nvim semantic color (`colors.*` in `lua/vercel/colors.lua`).

| Key | Dark | Light |
|-----|------|-------|
| background | `colors.background` `#000000` | `colors.background` `#FAFAFA` |
| foreground | `colors.foreground` `#EDEDED` | `colors.foreground` `#171717` |
| cursorColor | `colors.foreground` `#EDEDED` | `colors.foreground` `#171717` |
| selectionBackground | `colors.background_hover` `#1A1A1A` | `colors.background_hover` `#F2F2F2` |
| black | `colors.black` `#A1A1A1` | `colors.black` `#171717` |
| red | `colors.red` `#FF6166` | `colors.red` `#CB2A2F` |
| green | `colors.green` `#62C073` | `colors.green` `#297A3A` |
| yellow | `colors.amber` `#F2A20D` | `colors.amber` `#A35200` |
| blue | `colors.blue` `#52A8FF` | `colors.blue` `#0068D6` |
| purple | `colors.purple` `#BF7AF0` | `colors.purple` `#7820BC` |
| cyan | `colors.teal` `#0AC7B4` | `colors.teal` `#067A6E` |
| white | `colors.white` `#EDEDED` | `colors.white` `#4D4D4D` |
| tab.background | transparent `#00000000` | `colors.background` `#FAFAFAFF` |
| tabRow.background | `colors.background` `#000000FF` | `colors.background` `#FAFAFAFF` |
| tabRow.unfocusedBackground | `colors.background` `#000000FF` | `colors.background` `#FAFAFAFF` |

## Usage

Copy the variant you want:

1. Copy the raw content of `{{variant}}.jsonc` into `schemes` field of Windows Terminal's configuration file `settings.json`:

    ```json
    {
      // ...

      "schemes": [
        {
          "name": "Vercel Dark",

          "cursorColor": "#EDEDED", // colors.foreground
          "selectionBackground": "#1A1A1A", // colors.background_hover

          "background": "#000000",
          "foreground": "#EDEDED",

          "black": "#A1A1A1", // colors.black
          "red": "#FF6166",
          "green": "#62C073",
          "yellow": "#F2A20D", // colors.amber
          "blue": "#52A8FF",
          "purple": "#BF7AF0",
          "cyan": "#0AC7B4", // colors.teal
          "white": "#EDEDED", // colors.white

          "brightBlack": "#A1A1A1", // colors.black
          "brightRed": "#FF6166",
          "brightGreen": "#62C073",
          "brightYellow": "#F2A20D", // colors.amber
          "brightBlue": "#52A8FF",
          "brightPurple": "#BF7AF0",
          "brightCyan": "#0AC7B4", // colors.teal
          "brightWhite": "#EDEDED" // colors.white
        },
        {
          "name": "Vercel Light",

          "cursorColor": "#171717", // colors.foreground
          "selectionBackground": "#F2F2F2", // colors.background_hover

          "background": "#FAFAFA",
          "foreground": "#171717",

          "black": "#171717", // colors.black
          "red": "#CB2A2F",
          "green": "#297A3A",
          "yellow": "#A35200", // colors.amber
          "blue": "#0068D6",
          "purple": "#7820BC",
          "cyan": "#067A6E", // colors.teal
          "white": "#4D4D4D", // colors.white

          "brightBlack": "#171717", // colors.black
          "brightRed": "#CB2A2F",
          "brightGreen": "#297A3A",
          "brightYellow": "#A35200", // colors.amber
          "brightBlue": "#0068D6",
          "brightPurple": "#7820BC",
          "brightCyan": "#067A6E", // colors.teal
          "brightWhite": "#4D4D4D" // colors.white
        }
        // ... Other schemes
      ],

      // ...
    }
    ```

2. Copy the raw content of `{{variantTheme}}.jsonc` into `themes` field of Windows Terminal's configuration file `settings.json`:

    ```json
    {
      // ...

      "themes": [
        {
          "name": "Vercel Dark",
          "tab": {
            "background": "#000000FF",
            "showCloseButton": "always",
            "unfocusedBackground": null
          },
          "tabRow": {
            "background": "#000000FF",
            "unfocusedBackground": "#000000FF"
          },
          "window": {
            "applicationTheme": "dark"
          }
        },
        {
          "name": "Vercel Light",
          "tab": {
            "background": "#FAFAFAFF",
            "showCloseButton": "always",
            "unfocusedBackground": null
          },
          "tabRow": {
            "background": "#FAFAFAFF",
            "unfocusedBackground": "#FAFAFAFF"
          },
          "window": {
            "applicationTheme": "light"
          }
        }
        // ... Other themes
      ],

      // ...
    }
    ```

3. Choose the scheme and theme in Windows Terminal's settings:

    ```json
    {
      //...

      "profiles": {
        "defaults": {
          "colorScheme": "Vercel Dark",
          // ...
        }
      },

      // ...

      "theme": "Vercel Dark",

      //...
    }
    ```

4. Enjoy!
