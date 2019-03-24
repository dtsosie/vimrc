# vimrc

YouComplete Prequisites
sudo apt install build-essential cmake python3-dev vim-nox ruby-all-dev

git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

git clone https://github.com/dtsosie/vimrc.git ~/.vim

vim
:PluginInstall
:q

cd ~/.vim/bundle/command-t/ruby/command-t/ext/command-t
ruby extconf.rb
make

cd ~/.vim/bundle/YouCompleteMe
python3 install.py
