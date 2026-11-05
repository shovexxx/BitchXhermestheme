# BitchX Hermes Theme

Classic [BitchX](https://get-xsnow.de/) IRC client, reborn as Hermes
skins — black terminal, ANSI colours. Two switchable colourways; one
YAML themes **everything at once**: CLI, Ink TUI, and the desktop GUI
repaint live within ~a second.

- **`bitchx`** — the screenshot logo palette: magenta outline
  (`#FF00FF`), green→cyan core (`#00FF66`→`#00FFFF`), white dotted X,
  royal-blue status bar (`#0000CD`).
- **`bitchx-classic`** — the original teal palette: cyan channels
  (`#00C8C8`), teal borders (`#008080`), green prompt.

Switch any time: `hermes skin use bitchx` / `hermes skin use bitchx-classic`
(or `/skin` in-session).

If you know, you know.

## Install

```bash
mkdir -p ~/.hermes/skins
curl -fsSL https://raw.githubusercontent.com/shovexxx/BitchXhermestheme/main/bitchx.yaml \
  -o ~/.hermes/skins/bitchx.yaml
hermes config set display.skin bitchx
```

Or from a clone:

```bash
git clone https://github.com/shovexxx/BitchXhermestheme.git
cp BitchXhermestheme/bitchx.yaml ~/.hermes/skins/
hermes config set display.skin bitchx
```

For a named profile, drop the file in
`~/.hermes/profiles/<name>/skins/` instead.

## Revert

```bash
hermes config set display.skin default
```

## Palettes

**`bitchx` (logo):** black `#000000`, magenta outline `#FF00FF`,
green `#00FF66`, cyan `#00FFFF`, white `#FFFFFF`, yellow `#FFFF00`,
pink-red `#FF0066`, royal-blue status bar `#0000CD`.

**`bitchx-classic` (teal):** black `#000000`, cyan `#00C8C8`, teal
borders `#008080`, green `#00C800`, yellow `#E0E000`, red `#E00000`,
magenta numbers `#FF00FF`.

## License

MIT — see `LICENSE`.
