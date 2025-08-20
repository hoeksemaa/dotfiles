# dotfiles

Required Packages:
sudo apt install git stow

Instructions:
1) git clone directly into home
2) `stow vim`, then run `ls -al ~ | grep vimrc` to ensure symlinks were made
3) `git submodule update --init --recursive`
4) `stow tmux`, then run `ls -al ~ | grep tmux` to ensure symlinks were made
5) `tmux source tmux/.tmux.conf` 

To add submodule:
1) Navigate to vim/.vim/pack/plugins/start
2) git submodule add [clone url]
3) Module should be automatically loaded into vim, on next open

Reference links:
* https://alexpearce.me/2016/02/managing-dotfiles-with-stow/
* https://dev.to/iggredible/how-to-use-vim-packages-3gil

## submodule-specific instructions:
to get tagbar working, install exuberant ctags
`sudo apt install exuberant-ctags`

## thanks
special thanks to eshiman for pointing me to her repository: https://github.com/eshiman/dotfiles?tab=readme-ov-file
