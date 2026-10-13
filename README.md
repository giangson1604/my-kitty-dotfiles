# Kitty dotfiles

My [kitty](https://sw.kovidgoyal.net/kitty/) terminal setup. Colors come from the Nord theme,
applied with the [themes kitten](https://sw.kovidgoyal.net/kitty/kittens/themes/)
(`kitten themes`), which manages the `BEGIN_KITTY_THEME` block in `kitty.conf` and writes `current-theme.conf`.

| File | What it does |
|---|---|
| `kitty/kitty.conf` | Main config: theme include, cursor trail, grid layout, macOS behaviour |
| `kitty/blaze-nord.slang` | Cursor trail shader in Nord Frost blues |

## Install (macOS / Linux)

```bash
git clone https://github.com/YOUR_NAME/kitty-dotfiles.git ~/dotfiles/kitty-dotfiles
mv ~/.config/kitty ~/.config/kitty.bak          # back up the old config
ln -s ~/dotfiles/kitty-dotfiles/kitty ~/.config/kitty
```

Then quit kitty completely and open it again (a config reload may not pick up shader changes).

## Shortcuts

- `ctrl+shift+g` — switch to grid layout (square-ish panes)
- `ctrl+shift+l` — cycle layouts

## Credits

`blaze-nord.slang` is based on the Blaze cursor trail by chardskarth, ported to Slang by
Kovid Goyal, and distributed under the GPLv3 license (see the header in the file).
