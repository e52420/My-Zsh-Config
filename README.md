# My Zsh Config

## Zsh install with pulgins and themes

```bash
sudo pacman -S zsh
```

## Oh-my-zsh
```bash
sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```
## Plugins

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

```bash
 git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
```

## Powerlevel10k

```bash

git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

Now add powerlevel10k to zshrc adn the plugins too

```bash
ZSH_THEME="powerlevel10k/powerlevel10k"
```
```bash
plugins=(git zsh-syntax-highlighting zsh-completions zsh-autosuggestions)
```

And the aliases
```bash
alias sudo="doas"
alias cl="clear"
alias ls="exa -lah --icons --grid -s type"
alias l="exa --icons -l --grid -s type"
alias cat="bat"
```
