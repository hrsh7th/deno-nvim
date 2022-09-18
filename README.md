# deno-nvim

A plugin to improve deno experience

## Installation

using `packer.nvim`

```lua
use 'neovim/nvim-lspconfig'
use 'sigmasd/deno-nvim'
```

## Setup

This plugin automatically sets up nvim-lspconfig for deno for you, so don't do
that manually, as it causes conflicts.

Put this in your init.lua or any lua file that is sourced.<br>

Example config:

```lua
require("deno-nvim").setup({
  server = {
    on_attach = ...,
    capabilites = ...
  },
})
```

## Usage

<details>
  <summary>
	<b>deno test with code lens</b>
  </summary>
  (TODO)
</details>

<details>
  <summary>
	<b>auto complete import from deno registeries</b>
  </summary>
  (TODO)
</details>

# Important

There is currently a bug in neovim that prevent deno lsp form working 100 %
correctly see (https://github.com/neovim/neovim/pull/19967) and
(https://github.com/denoland/deno/issues/15786). If you're comfortable with
hacks you can use (https://github.com/neovim/neovim/pull/19773/files)
