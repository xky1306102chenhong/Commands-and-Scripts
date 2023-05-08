# editor选择
没有最好的兵器，只有称手的兵器。孙悟空适合金箍棒，八戒适合钉耙。

对我来说， vim是称手的兵器。

我喜欢工具的通用性，这样来带一种感觉，就好像搞数学只需要一张纸一支笔一样。

而emacs配置太个性化
# 配置文件
～/.vimrc

```

```

# 插件管理 Vundle
1. 下载Vundle
```
 git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
2. 将如下配置拷贝到.vimrc顶部
```
set nocompatible              " be iMproved, required
filetype off                  " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
" alternatively, pass a path where Vundle should install plugins
"call vundle#begin('~/some/path/here')

" let Vundle manage Vundle, required
Plugin 'VundleVim/Vundle.vim'

" The following are examples of different formats supported.
" Keep Plugin commands between vundle#begin/end.
" plugin on GitHub repo
Plugin 'tpope/vim-fugitive'
" plugin from http://vim-scripts.org/vim/scripts.html
" Plugin 'L9'
" Git plugin not hosted on GitHub
Plugin 'git://git.wincent.com/command-t.git'
" git repos on your local machine (i.e. when working on your own plugin)
Plugin 'file:///home/gmarik/path/to/plugin'
" The sparkup vim script is in a subdirectory of this repo called vim.
" Pass the path to set the runtimepath properly.
Plugin 'rstacruz/sparkup', {'rtp': 'vim/'}
" Install L9 and avoid a Naming conflict if you've already installed a
" different version somewhere else.
" Plugin 'ascenator/L9', {'name': 'newL9'}

" All of your Plugins must be added before the following line
call vundle#end()            " required
filetype plugin indent on    " required
" To ignore plugin indent changes, instead use:
"filetype plugin on
"
" Brief help
" :PluginList       - lists configured plugins
" :PluginInstall    - installs plugins; append `!` to update or just :PluginUpdate
" :PluginSearch foo - searches for foo; append `!` to refresh local cache
" :PluginClean      - confirms removal of unused plugins; append `!` to auto-approve removal
"
" see :h vundle for more details or wiki for FAQ
" Put your non-Plugin stuff after this line
```
3. 安装
```
：PluginInstall
```
4. 卸载
```
：PluginClean
```
5. 更新
```
：PluginUpdate
```

# 目录树
1. 下载nerdtree
```
~/.vim/bundle/Vundle.vim
```
2. 在.vimrc中添加
```
Plugin 'preservim/nerdtree'
```
3. 配置启动nerdtree的快捷键
```
".vimrc
map <C-n> :NERDTreeMirror<CR>
map <C-n> :NERDTreeToggle<CR>
```
