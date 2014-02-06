set nocompatible " Fuck VI... That's for grandpas.
filetype off
 
set rtp+=~/.vim/bundle/vundle/
call vundle#rc()
 
" Vundle let's you specify a plugin in a number of formats, but my favorite
" allows you to grab plugins straight off of github, just specify the bundle
" in the following format:
" Bundle 'githubUsername/repoName'
 
" Let vundle manage itself:
Bundle 'gmarik/vundle'
 
" Just a shitload of color schemes.
" https://github.com/flazz/vim-colorschemes#current-colorschemes
Bundle 'flazz/vim-colorschemes'
 
" Fuzzy finder -- absolutely must have.
Bundle 'kien/ctrlp.vim'
 
" Support for easily toggling comments.
Bundle 'tpope/vim-commentary'
 
" In addtion to the above plugins, you'll likely need some for individual
" non-standard syntaxes that aren't pre-bundled with vim. Here are some I use,
" these are required for me, but depending on what code you write, obviously
" this may differ for you.
 
" Proper JSON filetype detection, and support.
Bundle 'leshill/vim-json'
 
" vim already has syntax support for javascript, but the indent support is
" horrid. This fixes that.
Bundle 'pangloss/vim-javascript'
 
" vim indents HTML very poorly on it's own. This fixes a lot of that.
Bundle 'indenthtml.vim'
 
" I write markdown a lot. This is a good syntax.
Bundle 'tpope/vim-markdown'
 
" LessCSS -- I use this every day.
"Bundle 'groenewege/vim-less'
 
" Coffee-script syntax.
Bundle 'kchmck/vim-coffee-script'
 
" NERDtree plugin
Bundle 'scrooloose/nerdtree'
 
" We have to turn this stuff back on if we want all of our features.
filetype plugin indent on " Filetype auto-detection
set t_Co=256
syntax on " Syntax highlighting
set number

set tabstop=2
set shiftwidth=2
set softtabstop=2
set expandtab " use spaces instead of tabs.
set smarttab " let's tab key insert 'tab stops', and bksp deletes tabs.
set shiftround " tab / shifting moves to closest tabstop.
set autoindent " Match indents on new lines.
set smartindent " Intellegently dedent / indent new lines based on rules.
 
" We have VCS -- we don't need this stuff.
set nobackup " We have vcs, we don't need backups.
set nowritebackup " We have vcs, we don't need backups.
set noswapfile " They're just annoying. Who likes them?
 
" don't nag me when hiding buffers
set hidden " allow me to have buffers with unsaved changes.
set autoread " when a file has changed on disk, just load it. Don't ask.
 
" Make search more sane
set ignorecase " case insensitive search
set smartcase " If there are uppercase letters, become case-sensitive.
set incsearch " live incremental searching
set showmatch " live match highlighting
set hlsearch " highlight matches
set gdefault " use the `g` flag by default.
 
" allow the cursor to go anywhere in visual block mode.
set virtualedit+=block
 
" leader is a key that allows you to have your own "namespace" of keybindings.
" You'll see it a lot below as <leader>
let mapleader = ","
 
 
" So we don't have to press shift when we want to get into command mode.
nnoremap ; :
vnoremap ; :
 
" So we don't have to reach for escape to leave insert mode.
inoremap jf <esc>
inoremap jj <esc>
 
" create new vsplit, and switch to it.
noremap <leader>v <C-w>v
 
" bindings for easy split nav
nnoremap <C-h> <C-w>h
nnoremap <C-j> <C-w>j
nnoremap <C-k> <C-w>k
nnoremap <C-l> <C-w>l
 
" Use sane regex's when searching
nnoremap / /\v
vnoremap / /\v
 
" Clear match highlighting
noremap <leader><space> :noh<cr>:call clearmatches()<cr>
 
" Quick buffer switching - like cmd-tab'ing
nnoremap <leader><leader> <c-^>

 
" Visual line nav, not real line nav
" If you wrap lines, vim by default won't let you move down one line to the
" wrapped portion. This fixes that.
noremap j gj
noremap k gk
 
" Plugin settings:
" Below are some 'sane' (IMHO) defaults for a couple of the above plugins I
" referenced.
 
" Map the key for toggling comments with vim-commentary
nnoremap <leader>c <Plug>CommentaryLine
 
" Remap ctrlp to ctrl-t -- map it however you like, or stick with the
" defaults. Additionally, in my OS, I remap caps lock to control. I never use
" caps lock. This is highly recommended.
let g:ctrlp_map = '<c-p>'
 
" Let ctrlp have up to 30 results.
let g:ctrlp_max_height = 30
 
" NERDTree shortcut
nmap <leader>n :NERDTreeToggle<cr>
 
" Finally the color scheme. Choose whichever you want from the list in the
" link above (back up where we included the bundle of a ton of themes.)
colorscheme Monokai 
