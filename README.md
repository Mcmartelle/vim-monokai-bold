# vim-monokai-bold

I grew accustomed to the bold formatting of the light color scheme I use, Eiffel, and I wanted it in my prefered dark color scheme too.
Thus, monokai-bold.

* The colour palette from [sickill/vim-monokai](https://github.com/sickill/vim-monokai). 
* The original code is from [w0ng/vim-hybrid](https://github.com/w0ng/vim-hybrid).
* Other code is from [crusoexia/vim-monokai](https://github.com/crusoexia/vim-monokai).

Install
-------

### [vim-plug](https://github.com/junegunn/vim-plug)

    Plug 'mcmartelle/vim-monokai-bold'

### Manually

```bash
mkdir -p ~/.vim/colors
```
    
Download the `colors/monokai.vim` file from the repo to `~/.vim/colors`

Usage
-----

Copy below command to your `~/.vimrc`:

```VimL
syntax on
colorscheme monokai-bold
```

Terminal support
----------------

If you are using a terminal which support truecolor like **iterm2**, enable the gui color by adding below setting in `~/.vimrc` or `~/.vim/init.vim`

```VimL
set termguicolors
```

Otherwise, use below setting to activate the 256 color in terminal

```VimL
set t_Co=256  " vim-monokai now only support 256 colours in terminal.
```

coc.nvim support
--------------------

[coc.nvim](https://github.com/neoclide/coc.nvim) is a powerful completion engine, it brings *vs-code*'s experience into vim. *vim-monokai* fits it well.

Configuration
-------------

### Italic

By default the gui enables italic but terminal. They both can be configured.
    
If you are using a font support italic, paste below command in `.vimrc` to turn on terminal italic:

    let g:monokai_term_italic = 1
    let g:monokai_gui_italic = 1

Javascript
----------

For javascript development, it is recommended to install below plugins:

1. [vim-javascript](https://github.com/pangloss/vim-javascript), which provide features such as param syntax highlight, 
function assignment identifier highlight.

2. [vim-javascript-lib](https://github.com/crusoexia/vim-javascript-lib), which is the companion of _vim-javascript_, 
provide the popular javascript libraries key word highlight, such as [underscore](http://underscorejs.org/) and 
[Backbone](http://backbonejs.org/).

Typescript
----------

For better typescript highlight, it is recommend to install the [yats.vim](https://github.com/HerringtonDarkholme/yats.vim) syntax plugin.
