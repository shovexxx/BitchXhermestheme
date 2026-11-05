# BitchX Hermes Theme

Classic [BitchX](https://get-xsnow.de/) IRC client, reborn as a Hermes
skin — black terminal, ANSI colours, cyan channels, magenta highlights.
One YAML file themes **everything at once**: CLI, Ink TUI, and the
desktop GUI repaint live within ~a second.

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

## Palette

| Role | Colour |
|---|---|
| Background | `#000000` black |
| Text | `#c0c0c0` silver / `#ffffff` headings |
| Channels / accent | `#00c8c8` cyan, `#008080` teal borders |
| Prompt / tools / ok | `#00c800` green |
| Warnings / strings | `#e0e000` yellow |
| Errors | `#e00000` red |
| Numbers / highlights | `#ff00ff` magenta |

## License

MIT — see `LICENSE`.
