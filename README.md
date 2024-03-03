# Introduction

This repo is a fork form [jdhao](https://github.com/jdhao/nvim-config) but for my own
configuration for Linux, macOS, and Windows.

`init.lua` is the config entry point for terminal Nvim,
and `ginit.vim` is the additional config file for [GUI client of Nvim](https://github.com/neovim/neovim/wiki/Related-projects#gui).
(I'm using nvim-qt by myself)

# Install and setup

Autoscript to install on docs folder. 

# Features #

+ Plugin management via [Lazy.nvim](https://github.com/folke/lazy.nvim).
+ Code, snippet, word auto-completion via [nvim-cmp](https://github.com/hrsh7th/nvim-cmp).
+ Language server protocol (LSP) support via [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig).
+ Git integration via [vim-fugitive](https://github.com/tpope/vim-fugitive).
+ Better escaping from insert mode via [better-escape.vim](https://github.com/nvim-zh/better-escape.vim).
+ Ultra-fast project-wide fuzzy searching via [LeaderF](https://github.com/Yggdroot/LeaderF).
+ Faster code commenting via [vim-commentary](https://github.com/tpope/vim-commentary).
+ Faster matching pair insertion and jump via [delimitMate](https://github.com/Raimondi/delimitMate).
+ Smarter and faster matching pair management (add, replace or delete) via [vim-sandwich](https://github.com/machakann/vim-sandwich).
+ Fast buffer jump via [hop.nvim](https://github.com/phaazon/hop.nvim).
+ Powerful snippet insertion via [Ultisnips](https://github.com/SirVer/ultisnips).
+ Beautiful statusline via [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim).
+ File tree explorer via [nvim-tree.lua](https://github.com/nvim-tree/nvim-tree.lua).
+ Show search index and count with [nvim-hlslens](https://github.com/kevinhwang91/nvim-hlslens).
+ User-defined mapping hint via [which-key.nvim](https://github.com/folke/which-key.nvim).
+ Code highlighting via [nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter).
+ Beautiful nord colorscheme via [EdenEast/nightfox.nvim](https://github.com/EdenEast/nightfox.nvim).
+ Markdown writing and previewing via [vim-markdown](https://github.com/preservim/vim-markdown) and [markdown-preview.nvim](https://github.com/iamcco/markdown-preview.nvim).
+ LaTeX editing and previewing via [vimtex](https://github.com/lervag/vimtex)
+ Animated GUI style notification via [nvim-notify](https://github.com/rcarriga/nvim-notify).
+ Code formatting via [Neoformat](https://github.com/sbdchd/neoformat).
+ Undo management via [vim-mundo](https://github.com/simnalamburt/vim-mundo)
+ ......


# Shortcuts

Some of the shortcuts I use frequently are listed here. In the following shortcuts, `<leader>` represents ASCII character `,`.

| Shortcut          | Mode          | platform        | Description                                                              |
|-------------------|---------------|-----------------|--------------------------------------------------------------------------|
| `<leader>ff`      | Normal        | Linux/macOS/Win | Fuzzy file searching in a floating window                                |
| `<leader>fh`      | Normal        | Linux/macOS/Win | Fuzzy help file grepping in a floating window                            |
| `<leader>fg`      | Normal        | Linux/macOS/Win | Fuzzy project-wide grepping in a floating window                         |
| `<leader>ft`      | Normal        | Linux/macOS/Win | Fuzzy buffer tag searching in a floating window                          |
| `<leader>fb`      | Normal        | Linux/macOS/Win | Fuzzy buffer switching in a floating window                              |
| `<leader><Space>` | Normal        | Linux/macOS/Win | Remove trailing white spaces                                             |
| `<leader>v`       | Normal        | Linux/macOS/Win | Reselect last pasted text                                                |
| `<leader>ev`      | Normal        | Linux/macOS/Win | Edit Nvim config in a new tabpage                                        |
| `<leader>sv`      | Normal        | Linux/macOS/Win | Reload Nvim config                                                       |
| `<leader>st`      | Normal        | Linux/macOS/Win | Show highlight group for cursor text                                     |
| `<leader>q`       | Normal        | Linux/macOS/Win | Quit current window                                                      |
| `<leader>Q`       | Normal        | Linux/macOS/Win | Quit all window and close Nvim                                           |
| `<leader>w`       | Normal        | Linux/macOS/Win | Save current buffer content                                              |
| `<leader>y`       | Normal        | Linux/macOS/Win | Copy the content of entire buffer to default register                    |
| `<leader>cl`      | Normal        | Linux/macOS/Win | Toggle cursor column                                                     |
| `<leader>cd`      | Normal        | Linux/macOS/Win | Change current working directory to to the dir of current buffer         |
| `<space>t`        | Normal        | Linux/macOS/Win | Toggle tag window (show project tags in the right window)                |
| `<leader>gs`      | Normal        | Linux/macOS/Win | Show Git status result                                                   |
| `<leader>gw`      | Normal        | Linux/macOS/Win | Run Git add for current file                                             |
| `<leader>gd`      | Normal        | Linux/macOS/Win | Run git diff for current file                                            |
| `<leader>gc`      | Normal        | Linux/macOS/Win | Run git commit                                                           |
| `<leader>gpl`     | Normal        | Linux/macOS/Win | Run git pull                                                             |
| `<leader>gpu`     | Normal        | Linux/macOS/Win | Run git push                                                             |
| `<leader>gl`      | Normal/Visual | Linux/macOS/Win | Get perm link for current/visually-select lines
| `<leader>gb`      | Normal        | macOS           | Browse current git repo in browser
| `<F9>`            | Normal        | Linux/macOS/Win | Compile&run current source file (for C++, LaTeX, Lua, Python)            |
| `<F11>`           | Normal        | Linux/macOS/Win | Toggle spell checking                                                    |
| `<F12>`           | Normal        | Linux/macOS/Win | Toggle paste mode                                                        |
| `\x`              | Normal        | Linux/macOS/Win | Close location or quickfix window                                        |
| `\d`              | Normal        | Linux/macOS/Win | Close current buffer and go to previous buffer                           |
| `{count}gb`       | Normal        | Linux/macOS/Win | Go to buffer `{count}` or next buffer in the buffer list.                |
| `{operator}iB`    | Normal        | Linux/macOS/Win | Operate in the whole buffer, `{operator}` can be `v`, `y`, `c`, `d` etc. |
| `Alt-k`           | Normal        | Linux/macOS/Win | Move current line or selected lines up                                   |
| `Alt-j`           | Normal        | Linux/macOS/Win | Move current line or selected lines down                                 |
| `Alt-m`           | Normal        | macOS/Win       | Markdown previewing in system browser                                    |
| `Alt-Shift-m`     | Normal        | macOS/Win       | Stopping Markdown previewing in system browser                           |
| `ob`              | Normal/Visual | macOS/Win       | Open link under cursor or search visual selection                        |
| `ctrl-u`          | Insert        | Linux/macOS/Win | Turn word under cursor to upper case                                     |
| `ctrl-t`          | Insert        | Linux/macOS/Win | Turn word under cursor to title case                                     |
| `jk`              | Insert        | Linux/macOS/Win | Return to Normal mode without lagging                                    |

# Custom commands

In addition to commands provided by various plugins, I have also created some custom commands for personal use.

| command    | description                                                             | example                        |
|------------|-------------------------------------------------------------------------|--------------------------------|
| `Redir`    | capture command output to a tabpage for easier inspection.              | `Redir hi`                     |
| `Edit`     | edit multiple files at the same time, supports globing                  | `Edit *.vim`                   |
| `Datetime` | print current date and time or convert Unix time stamp to date and time | `Datetime 12345` or `Datetime` |


# Further readings

More info are in base jdhao's repo. 
