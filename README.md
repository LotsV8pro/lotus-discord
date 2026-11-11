<p align="center">
  <img src="https://img.shields.io/badge/Vencord-141218?style=for-the-badge&logo=discord&logoColor=C4A8E2"/>
  <img src="https://img.shields.io/badge/Lotus_Purple-141218?style=for-the-badge&logo=codeforces&logoColor=C4A8E2"/>
</p>

<h1 align="center">Lotus Discord</h1>

A purple glass theme for Discord, loaded through Vencord. It uses the same
palette as the other Lotus repos: dark background, lavender accents, translucent
panels.

The palette is the same one used by
[Lotus-Arch](https://github.com/LotsV8pro/Lotus-Arch), so a screenshot of
Discord next to the desktop does not clash.

## Install

Vencord reads user themes from `~/.config/Vencord/themes/`.

```bash
mkdir -p ~/.config/Vencord/themes
curl -fsSL https://raw.githubusercontent.com/LotsV8pro/lotus-discord/master/themes/lotus-purple.theme.css \
  -o ~/.config/Vencord/themes/lotus-purple.theme.css
```

Then open Discord, go to Settings, Vencord, Themes, and enable `lotus-purple`.

Vesktop uses the same Vencord plugin and the same folder.

## What it changes

- The window, sidebar, chat and member list get a translucent purple layer over
  a blur of the background.
- Buttons, inputs, search, embeds, reactions and code blocks follow the accent
  and border colours.
- Context menus, modals, tooltips and the call view are restyled.
- Scrollbars get a thin accent thumb and a transparent track.

Class names in Discord change every few weeks. The selectors here match the
stable part of the generated names (`[class*="base_"]`) instead of a full hash,
so a Discord update usually does not break the theme.

## Palette

| Token | Hex |
|---|---|
| Accent | `#C4A8E2` |
| Accent dim | `#8C7AA6` |
| Accent dark | `#383048` |
| Text | `#D8D0E8` |
| Text dim | `#887898` |
| Background | `#141218` |
| Background alt | `#1C1A22` |
| Background light | `#282430` |

The variables live at the top of `themes/lotus-purple.theme.css`. Changing them
there changes the whole theme.

## Compatibility

- Discord with Vencord
- Vesktop, which ships Vencord

It does not work with BetterDiscord without renaming the file and adapting the
metadata block.

## Related repos

- [lotus-spotify](https://github.com/LotsV8pro/lotus-spotify): the same palette for Spotify
- [lotus-steam](https://github.com/LotsV8pro/lotus-steam): the same palette for Steam
- [Lotus-Arch](https://github.com/LotsV8pro/Lotus-Arch): the desktop it matches

## License

MIT.
