<p align="center">
  <img src="https://img.shields.io/badge/Vencord-141218?style=for-the-badge&logo=discord&logoColor=C4A8E2"/>
  <img src="https://img.shields.io/badge/Lotus_Purple-141218?style=for-the-badge&logo=codeforces&logoColor=C4A8E2"/>
  <img src="https://img.shields.io/badge/Lotus_Pastel-2B2740?style=for-the-badge&logo=codeforces&logoColor=D8BBFF"/>
</p>

<h1 align="center">Lotus Discord</h1>

Themes for Discord, loaded through Vencord. They follow the same visual
language as the other Lotus repos: deep purple backgrounds, lavender accents,
soft edges, pastel colours. The palette matches
[Lotus-Arch](https://github.com/LotsV8pro/Lotus-Arch), so Discord and the
desktop do not clash.

Two themes ship here:

- **Lotus Purple** — the original purple glassmorphism theme.
- **Lotus Pastel (Caelestia)** — a pastel violet/pink build with a custom
  animated lotus on the Home button, no filled background on selected items,
  and the window controls hidden (niri handles those).

## Install

Vencord reads user themes from `~/.config/Vencord/themes/`.

```bash
mkdir -p ~/.config/Vencord/themes
curl -fsSL https://raw.githubusercontent.com/LotsV8pro/lotus-discord/master/themes/lotus-purple.theme.css \
  -o ~/.config/Vencord/themes/lotus-purple.theme.css
curl -fsSL https://raw.githubusercontent.com/LotsV8pro/lotus-discord/master/themes/caelestia.theme.css \
  -o ~/.config/Vencord/themes/caelestia.theme.css
```

Then open Discord: Settings -> Vencord -> Themes. Enable `lotus-purple` and/or
`caelestia`. The Home-button lotus needs `caelestia` enabled and its SVGs next
to the theme file (in Vencord's theme folder or under `themes/assets/` in this
repo).

Vesktop uses the same Vencord plugin and the same folder.

## What they change

- Window, sidebar, chat and member list get a translucent purple layer.
- Buttons, inputs, search, embeds, reactions and code blocks follow the accent
  and border colours.
- Context menus, modals, tooltips and the call view are restyled.
- Scrollbars get a thin accent thumb and a transparent track.

`caelestia` adds:

- Pastel violet/pink palette: background `#221b33`, text `#efe9f7`, accents
  from `--purple-*`, rosa `#f49ac4`, mint `#9ee0c4`.
- Home button replaced by a lotus. On hover the centre petal rises from the
  bottom and the others open like a fan, slowly. When selected it stays open
  and static, with no filled background.
- Window controls hidden: niri already draws its own.

Class names in Discord change every few weeks. The selectors match the stable
part of generated names (`[class*="base_"]`) instead of a full hash, so a
Discord update usually does not break the themes.

## Palette — Lotus Purple

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

## Palette — Lotus Pastel (Caelestia)

| Token | Hex |
|---|---|
| Main background | `#221b33` |
| Surface | `#2e2840` |
| Text | `#efe9f7` |
| Accent / lotus | `#c4a8e2` |
| Accent bright | `#dcc0ff` |
| Rosa (dnd) | `#f49ac4` |
| Mint (online) | `#9ee0c4` |
| Violet (streaming) | `#bfb8ff` |

The variables live at the top of each theme file. Changing them there changes
the whole theme.

## Compatibility

- Discord with Vencord
- Vesktop, which ships Vencord

They do not work with BetterDiscord without renaming the file and adapting the
metadata block.

## Related repos

- [lotus-spotify](https://github.com/LotsV8pro/lotus-spotify): the same palette for Spotify
- [lotus-steam](https://github.com/LotsV8pro/lotus-steam): the same palette for Steam
- [Lotus-Arch](https://github.com/LotsV8pro/Lotus-Arch): the desktop it matches

## License

MIT.
