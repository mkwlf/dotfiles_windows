# WSL dotfiles
Ubuntu 20.04 WSL dotfiles

## Installation
1. clone this repo `git clone git@github.com:mkwlf/dotfiles_windows.git ~/.dotfiles`
2. link git config `ln -s ~/.dotfiles/git/gitconfig ~/.gitconfig`
3. copy and edit `.gitconfig.local`: `cp ~/.dotfiles/git/gitconfig.local && vim ~/.gitconfig.local`
4. link vim config `ln -s ~/.dotfiles/vim/vimrc ~/.vimrc`

### zsh
1. install [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)
2. install `thefuck`: `sudo apt-get install thefuck`
3. remove zshrc: `rm ~/.zshrc`
4. link zshconfig `ln -s ~/.dotfiles/zsh/zshrc ~/.zshrc`
5. install [starship](https://github.com/starship/starship)

### environments
1. install [nvm](https://github.com/nvm-sh/nvm) for node version management
2. install [pyenv](https://github.com/pyenv/pyenv) for python version management
3. install [phpenv](https://github.com/phpenv/phpenv) via installer for php version management


#### phpenv issues
Forgot most of the steps to install php 8.x via phpenv. 
Try to install a php version for example via `phpenv install 8.1.1` and resolve missing package issues as they come.
If you get stuck make use of the `-v` option on installing. This way I was able to make out the issue, that autoconf was
not installed: `sudo apt-get install autoconf`.


