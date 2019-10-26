# vimrc

YouComplete Prequisites

# Ubuntu

sudo apt install build-essential cmake python3-dev vim-nox ruby-all-dev

# OSX

brew install macvim

# Main install
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

git clone https://github.com/dtsosie/vimrc.git ~/.vim/vimrc

ln -sf ~/.vim/vimrc/.vimrc ~/.vimrc

vim
:PluginInstall
:q

cd ~/.vim/bundle/command-t/ruby/command-t/ext/command-t

ruby extconf.rb

make

cd ~/.vim/bundle/YouCompleteMe

python3 install.py
pip3 install --user --upgrade pynvim
