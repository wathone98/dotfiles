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

### Optional
Install xclip for vim-tmux yank (Required only for ubuntu non-wsl)
```
sudo apt install xclip
```

## Pushing to Git
Remember to use `gitpath` instead of `git` for git commands

## Vim Shortcuts

For moving and editing in Vim
| Function											| Shortcut					|
| ----------------							| -------------			|
| Delete line										| `dd`							|
| Delete word										| `dw` / `dW`				|
| Select line										| `Shift`+`v`				|
| Cut line											| `D`								|
| Copy													|	`y`								|
| Paste													| `<X>`+`p`					|
| Insert mode										| `i` / `a`					|
| Insert new line								| `o`								|
| Undo / Redo										| `u` / `Ctrl`+`r`	|
| Find XXX below / on top				| `/`/`?` + `XXX`		|
| Change till certain X					| `cfX`							|
| Go through searches						| `n` / `N`					|
| Apply same change as previous	| `<X>` + `.`				|
| Go to next / previous words		| `w`/`e`/`b`				|
| Go to start / end of line			| `0` / `$`					|
| Go to top / bottom						| `gg` / `G`				|
| Go to line X									| `:<X>`/ `<X>gg`		|
| Move X lines up / down				| `<X>``k` / `j`		|
| Centre the screen							| `zz`							|

For Surround in Vim
* v = visual, e = end, s = surround
* If start of bracket is used, a space buffer is inserted.
| Function											| Shortcut					|
| ----------------							| -------------			|
| Surround with bracket					| `ves}`						|
| Delete surrounding bracket		| `ds}`							|

For Nerdtree in Vim
| Function											| Shortcut					|
| ----------------							| -------------			|
| Open tree											| `Ctrl`+`T`				|
| Open new tab									| `T`								|
| Switch windows								| `Ctrl`+`ww`				|
| Switch tabs										| `Ctrl`+`h`/`l`		| 
| Edit file											| `m`								|

For split screens
| Function											| Shortcut					|
| ----------------							| -------------			|
| Horizontal split							| `Ctrl`+`b` `"`		|
| Vertical split								| `Ctrl`+`b` `%`		|
| Kill window										| `Ctrl`+`d`				|
| Navigate windows							| `Ctrl`+`b` `hjkl`	|
| Resize windows								| `Alt`+`hjkl`			|

