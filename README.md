# vimrc

YouComplete Prequisites

# Ubuntu
###### Untested: Probably need to change /usr/local/bin/pip3 to just pip3 at the end

sudo apt install build-essential cmake python3-dev vim-nox ruby-all-dev

# OSX

brew install vim cmake

vim ~/.bash_profile

```
export EDITOR=/usr/local/bin/vim
alias vi="$EDITOR"
alias vim="$EDITOR"
```

# Main install
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

git clone https://github.com/dtsosie/vimrc.git ~/.vim/vimrc

ln -sf ~/.vim/vimrc/.vimrc ~/.vimrc

vim

```
:PluginInstall
:q
```

cd ~/.vim/bundle/command-t/ruby/command-t/ext/command-t

ruby extconf.rb

make

cd ~/.vim/bundle/YouCompleteMe

python3 install.py

/usr/local/bin/pip3 install --user --upgrade pynvim
