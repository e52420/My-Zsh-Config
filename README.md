# ayoub-elassri-zsh

#Zsh install with pulgins and themes

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
```bash
 git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
```

Starship prompt ->
```bash
sh -c "$(curl -fsSL https://starship.rs/install.sh)"
```

Now add all the plugins to the .zshrc file. For the starship prompt add this

```bash
eval "$(starship init zsh)"
```
