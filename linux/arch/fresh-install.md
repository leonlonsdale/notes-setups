# Package installs

## Get Homebrew

```web
https://homebrew.sh
```

## Check for updates

```bash
sudo pacman -Syu
```

## Get packages

### Utility and apps

```bash
sudo pacman -S yay wayland hyprland swaync zsh starship --needed
```

### GUI Software

```bash
sudo pacman -S discord bitwarden obsidian --needed
```

### Utils from Brew

```bash
brew install exa fastfetch fd jq zoxide zsh-autosuggestions zsh-syntax-highlighting yazi
```

### Language Stuff from Brew

#### Python

```bash
brew install python uv basedpyright ruff
```

#### Golang

```bash
brew install go goimports golangci-lint golangci-lint-langserver gopls
```

#### Web stuff

```bash
brew install typescript biome pgformatter prettier sql-language-server tailwindcss-language-server typescript-language-server vscode-langservers-extracted oven-sh/bun/bun node
```

#### Misc

```bash
brew install gh git marksman stylua yaml-language-server 
```
