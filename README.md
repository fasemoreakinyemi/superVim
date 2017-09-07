# superVim
## Modify Vim for superior capabilities
### Caveat: This idea and instruction is based on the information from this website 'https://realpython.com/blog/python/vim-and-python-a-match-made-in-heaven/' and this git page 'https://github.com/Valloric/YouCompleteMe#python-semantic-completion'

Instructions
- Install the vundle plugin manager 
```
$ git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
- Download the vimrc file into your home directory
```
wget https://raw.githubusercontent.com/theNNvader/superVim/master/vimrc
```

- Rename the file into a vim configuration file
```
$ mv vimrc .vimrc
```
- Open vim and run this code to install all the plugins in the configuration file
```
:PluginInstall
```
- Install YoucompleteMe for autocompletion
  ```
  cd ~
  mkdir ycm_build
  cd ycm_build
  cmake -G "Unix Makefiles" . ~/.vim/bundle/YouCompleteMe/third_party/ycmd/cpp
  cmake --build . --target ycm_core --config Release
  ```
Note: I have modified the information from the reference website to generate the vimrc file.
That's it we are done!
  

