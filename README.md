# Neovim
init.vim for neovim

## Install Neovim
Install neovim: https://github.com/neovim/neovim/wiki/Installing-Neovim

To start Neovim, run `nvim` (not `neovim`).


## Config (vimrc)
Put [init.vim](init.vim) in `~/.config/nvim`, or simply clone this repo:

```
git clone https://github.com/huwan/nvim.git ~/.config/nvim
```

## Install the Vim-plug Plugin Manager

```
 curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

[init.vim](init.vim) is configured to automatically install missing plugins on startup, or you can reload `init.vim` and execute `:PlugInstall` mannually after install new plugin(s).

NOTE: The following error message will be displayed at first nvim startup. Just ignore it. vim-anyfold plugin will be automatically installed and fix this issue.
```
Error detected while processing FileType Autocommands for "*":
E492: Not an editor command: AnyFoldActivate
Press ENTER or type command to continue
```

## Launch nvim
Launch `nvim`, the plugin will be ready for use.

## (Optional) Set vim alternative 
Add alias in .bashrc, .bash_aliases, or .bash_profile.

```
alias vi='nvim'
alias vim='nvim'
```

Or add vim alternative for nvim

```
sudo update-alternatives --install /usr/bin/vi vi /usr/bin/nvim 60
sudo update-alternatives --config vi
sudo update-alternatives --install /usr/bin/vim vim /usr/bin/nvim 60
sudo update-alternatives --config vim
```
