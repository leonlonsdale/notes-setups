# Package installs

## Get Homebrew

```web
https://brew.sh
```

## Check for updates

```bash
sudo pacman -Syu
```

## Get packages

### pacman

#### Terminal & CLI

```bash
sudo pacman -S yay wayland hyprland swaync zsh starship stow ghostty eza fastfetch fd jq zoxide zsh-autosuggestions zsh-syntax-highlighting yazi gh git ttf-jetbrains-mono-nerd --needed --noconfirm
```

### GUI Software

```bash
sudo pacman -S discord bitwarden obsidian --needed --noconfirm
```
### brew

#### Language Stuff with Brew

```bash
brew install typescript biome pgformatter prettier sql-language-server tailwindcss-language-server typescript-language-server vscode-langservers-extracted oven-sh/bun/bun node go goimports golangci-lint golangci-lint-langserver gopls python uv basedpyright ruff marksman stylua yaml-language-server
npm i -g @olrtg/emmet-language-server
```

# Change Shell

```bash
chsh -s "$(which zsh)"
```

# Dotfiles

```bash
cd ~
git clone --depth 1 --branch main https://github.com/leonlonsdale/dots.git -d
cd dots
stow .
```

restart the terminal

```bash
source ~/.zshrc
```
