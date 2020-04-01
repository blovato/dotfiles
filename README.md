# dotfiles
settings and configurations for my machine
git setup is based on [this guide](https://developer.atlassian.com/blog/2016/02/best-way-to-store-dotfiles-git-bare-repo/).

## Setup on a new machine
1. Install iTerm: `$ brew install iterm2`
1. Install zsh: `$ brew install zsh`
1. Install Oh-my-zsh: `$ sh -c "$(curl -fsSL
   https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
1. Install vim-plug: `$ curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim`
1. Install nvm: `$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash`
1. Clone dotfiles repo: `$ git clone --bare https://github.com/blovato/dotfiles $HOME/.dotfiles`
1. Alias dotfiles: `$ alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'`
1. Resolve conflicts: `$ dotfiles checkout` (resolve conflicts if they arise)
1. Configure dotfiles:`$ dotfiles config --local status.showUntrackedFiles no`
1. Install vim plugins: In vim run `:PlugInstall`
