# Zsh

## Alias (optional)

These alias' are my personal preference and are optiona.

```bash
alias cl="clear" # faster clear
alias ls="eza --icons=always" # use eza for ls
alias cd="z" # use zoxide for cd

alias bfi="brew bundle --file=~/.config/homebrew/Brewfile"
alias bfc="brew bundle dump --file=~/.config/homebrew/Brewfile"
alias bfr='rm -f ~/.config/homebrew/Brewfile && brew bundle dump --file=~/.config/homebrew/Brewfile'
```

## Enabling Apps

Note, the following will not work unless the packages have been installed. See Linux or MacOS fresh install documents.

### Enabling Homebrew

Add the following to the start of the `.zshrc`:

```bash
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv zsh)"
```

### Enabling Starship

Add the following to the start of `.zshrc`. This is optional. Without this line you simply add the starship.toml to `~/.config`

```bash
export STARSHIP_CONFIG=~/.config/starship/starship.toml
```

Add the following to the end (required)

```bash
eval "$(starship init zsh)"
```

### Enabling Zoxide

Add the following to the end of the file

```bash
eval "$(zoxide init zsh)"
```

### Enabling zsh auto suggestions and syntax highlighting

Add to the end of `.zshrc`

```bash
source /opt/homebrew/share/zsh-autosuggestions/zsh-autosuggestions.zsh
source /opt/homebrew/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh

# History

HISTFILE=$HOME/.zhistory
SAVEHIST=1000
HISTSIZE=999
setopt share_history
setopt hist_expire_dups_first
setopt hist_ignore_dups
setopt hist_verify

bindkey '^[[A' history-search-backward
bindkey '^[[B' history-search-forward
```


## Apply Changes

Exit your text editor and type:

```bash
source ~/.zshrc
```
