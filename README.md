## Setup

Install ZSH
```
sudo apt install zsh
```

Change Shell to ZSH
```
chsh -s $(which zsh)
```

Install Vim plugin manager
```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Clone and check out bare repo, set directories
```
git clone --bare --recursive https://github.com/wathone98/dotfiles.git $HOME/dotfiles
git --git-dir=$HOME/dotfiles --work-tree=$HOME checkout
```

Use zsh and update plugins
```
zsh
source ~/.zshrc
update
```

## Optional
Install xclip for vim-tmux yank (Required only for ubuntu non-wsl)
```
sudo apt install xclip
```

## Shortcuts

For moving and editing
| Function					| Shortcut			|
| ----------------	| ------------- |
| Delete line				| `d d`					|
| Insert mode				| `i` / `a`			|
| Insert new line		| `o`						|
