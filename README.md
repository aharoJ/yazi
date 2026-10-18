# yazi-config

Yazi configuration for macOS, with Vim-style keys and clipboard helpers.

Natural sorting with folders first, hidden files off and a 1:4:3 pane layout.
Neovim, VS Code, Modern CSV and system openers, with the built-in theme defaults.

- `q`: quit; `Q`: skip the cwd file used by shell wrappers.
- `Enter`: open the hovered file; `Space`: toggle selection; `owp`: open-with picker.
- `cc`: copy raw hovered file contents.
- `cC`: contents with headers (`copy-contents.sh`), including directory contents.
- `ct`: directory trees or filenames (`copy-tree.sh`); `cp`: paths (`copy-paths.sh`).

Requires Yazi and eza; the helpers use macOS `pbcopy`.
Back up your current config, then run from this repo:

```sh
mkdir -p ~/.config/yazi/scripts
cp yazi.toml keymap.toml theme.toml ~/.config/yazi/
cp scripts/copy-*.sh ~/.config/yazi/scripts/
chmod +x ~/.config/yazi/scripts/copy-*.sh
```

Quit and reopen Yazi after changing the config.

MIT. See [LICENSE](LICENSE).
