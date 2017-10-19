<img src="https://neovim.io/images/logo@2x.png" width="100">

```
shell> brew install neovim
shell> curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

`.vimrc`
```vim
call plug#begin('~/.vim/plugged')
Plug 'altercation/vim-colors-solarized'
Plug 'vim-airline/vim-airline'
Plug 'vim-airline/vim-airline-themes'
Plug 'tpope/vim-commentary'
Plug 'scrooloose/nerdtree'
Plug 'mattn/emmet-vim'
call plug#end()

syntax enable
set background=dark
" set background=light
let g:solarized_termcolors=256
colorscheme solarized

let g:airline_powerline_fonts = 1
let g:airline_theme='solarized'
set laststatus=2

autocmd vimenter * NERDTree
autocmd bufenter * if (winnr("$") == 1 && exists("b:NERDTree") && b:NERDTree.isTabTree()) | q | endif

set number
set cursorline
```

- `:PlugInstall`
- `:help commentary`

```
shell> nvim scp://192.168.88.18/~/myfile.txt
```

#### :books: 參考網站：
- https://github.com/neovim/neovim
- https://github.com/mattn/emmet-vim
- https://github.com/scrooloose/nerdtree
- https://github.com/vim-airline/vim-airline-themes
