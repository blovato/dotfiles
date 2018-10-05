# dotfiles
settings and configurations for my machine

## Setup on a new machine
1. `$ git clone --bare https://github.com/blovato/dotfiles $HOME/.dotfiles`
2. `$ alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'`
3. `$ dotfiles checkout` (resolve conflicts if they arise)
4. `$ dotfiles config --local status.showUntrackedFiles no`
