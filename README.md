# nvim-config
Configuration for [Neovim](https://github.com/neovim/neovim) documented for easier use to copy configurations across systems.

## Plugins
- [vim-plug](https://github.com/junegunn/vim-plug)
- [coc.nvim](https://github.com/neoclide/coc.nvim)
- [fzf.vim](https://github.com/junegunn/fzf.vim)
- [lightline.vim](https://github.com/itchyny/lightline.vim)
- [vim-rooter](https://github.com/airblade/vim-rooter)

## CoC Language Servers
- [C/C++/Objective-C](https://github.com/clangd/coc-clangd)
    - Requires `clangd`. Check for local `clangd` first before downloading.
    - Generate `compile_commands.json` for each project.
- [Python](https://github.com/fannheyward/coc-pyright)
- [Javascript/Typescript](https://github.com/neoclide/coc-tsserver)
- [JSON](https://github.com/neoclide/coc-json)

## CoC Extensions
- [Autopair](https://github.com/neoclide/coc-pairs)

## Initialization
1. Install [vim-plug](https://github.com/junegunn/vim-plug).
1. Copy `init.vim` into the specified config folder for neovim. Create the config directory using the following command through neovim:
``` 
:call mkdir(stdpath('config'),'p')
```
1. Call `:PlugInstall` inside neovim to install all the plugins.
1. Install nodejs in order for the coc.nvim plugin to run.
1. Install neovim extensions:
```
:CocInstall coc-clangd coc-pyright coc-tsserver coc-json
```

