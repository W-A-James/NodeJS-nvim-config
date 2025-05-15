# nvim_lua_setup

## Setup

Requires nvim >= v0.10.0

- Fork this repository (I make changes to this frequently, so do not treat this as a stable repository)
- Install [neovim](git@github.com:neovim/neovim.git) and locate the install directory. On Unix systems this should be at `~/.config/nvim`
- Install [lua](https://www.lua.org/download.html) and ensure the lua binary is in your system `$PATH`
- Clone your fork as follows `git clone <fork url> ~/.config/nvim`. This will replace your neovim configuration, so back up those settings if you would like to return to them
- It's not required to install packer separately as this config bootstraps it for you
- Open `nvim` and run `:PackerInstall` to install plugins
- Refer to [nvim-lspconfig's language server configurations document](https://github.com/neovim/nvim-lspconfig/blob/master/doc/server_configurations.md) to install desired language servers

## Repository Layout

### `init.lua`

Contains preferences and theme setup as well as some useful autocommands tailored to the languages that I normally work with (Rust, OCaml) and imports the other lua files

### `lua/plugins.lua`

Uses [packer](https://github.com/wbthomason/packer.nvim) to install plugins and conditionally 
bootstraps the packer installation.

### `lua/dap`

Contains configuration for debugging capabilities via the [Debug Adapter
Protocol](https://github.com/mfussenegger/nvim-dap).

### `lua/luasnip`

Contains snippet configuration.

### `lua/nvim-tree`

Contains configuration for [nvim-tree](https://github.com/nvim-tree/nvim-tree.lua).

### `lua/orgmode`

Contains confguration for [nvim-orgmode](https://github.com/nvim-orgmode/orgmode).

### `lua/treesitter`

Contains treesitter configuration.

### `lua/lsp`

Sets up language servers and mappings for code suggestions and completion

### `lua/lsp`

Sets up language servers and mappings for code suggestions and completion

### `lua/config/completion.lua`

Sets up autocompletion sources with [Treesitter](https://github.com/nvim-treesitter/nvim-treesitter)

### `lua/config/editor.lua`

Contains basic vim option configuration.

### `lua/config/keymap.lua`

Contains keymap configuration.

### `lua/config/theme.lua`

Theme configuration.

### `lua/config/utils.lua`

Shared utility functions.

