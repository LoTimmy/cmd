<img src="https://neovim.io/images/logo@2x.png" width="100">

```
shell> brew install neovim
shell> pip2 install neovim
shell> pip3 install neovim
shell> sudo gem install neovim
```

`VimPlug`
```
shell> curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

`~/.config/nvim/init.vim`
```vim
call plug#begin('~/.vim/plugged')
Plug 'altercation/vim-colors-solarized'
Plug 'vim-airline/vim-airline'
Plug 'vim-airline/vim-airline-themes'
Plug 'tpope/vim-commentary'
Plug 'tpope/vim-markdown'
Plug 'mattn/emmet-vim'
Plug 'pangloss/vim-javascript'
Plug 'easymotion/vim-easymotion'
Plug 'prettier/vim-prettier', {
  \ 'do': 'yarn install',
  \ 'for': ['javascript', 'typescript', 'css', 'less', 'scss', 'json', 'graphql'] }
call plug#end()

set t_Co=256
syntax enable
set background=dark
" set background=light
let g:solarized_termcolors=256
colorscheme solarized

let g:airline_powerline_fonts = 1
let g:airline_theme='solarized'
set laststatus=2

let mapleader = ","
nmap <Leader>p <Plug>(Prettier)

map <Leader>l <Plug>(easymotion-lineforward)
map <Leader>j <Plug>(easymotion-j)
map <Leader>k <Plug>(easymotion-k)
map <Leader>h <Plug>(easymotion-linebackward)

set number
set cursorline
set mouse-=a

au BufNewFile,BufRead Brewfile setf brew
autocmd FileType brew setlocal commentstring=#\ %s
```

- `:CheckHealth`
- `:PlugInstall`
- `:PlugClean`
- `:PlugStatus`
- `:Prettier`
- `:help commentary`

```
set noai
set nocin
set nosi
set inde=

noautoindent
nocindent
nosmartindent
indentexpr
```

```
shell> nvim scp://192.168.88.18/~/myfile.txt
```

#### :books: 參考網站：
- https://github.com/neovim/neovim
- https://github.com/junegunn/vim-plug
- https://github.com/mattn/emmet-vim
- https://github.com/scrooloose/nerdtree
- https://github.com/vim-airline/vim-airline-themes
