# My Neovim Colorscheme

This is a Neovim colorscheme based on the [mini.base16](https://vimcolorschemes.com/echasnovski/mini.base16) plugin.

## Installation

With Lazy:

```bash
return {
  {
    "TSawyer87/tokyo_drift",
    lazy = false,
    priority = 1000,
    config = function()
      -- You can set the colorscheme here if you want it to be automatic
      vim.cmd.colorscheme("tokyo_drift")
    end,
  },
  -- Other plugins...
}
```

-   `lazy = false` ensures the colorscheme is loaded immediately, which is typically desired for colorschemes to apply the theme upon startup.
-   `lazy = true` can be used if you want to load the colorscheme on demand, but this might require additional setup like a command or keymap to activate it manually.

Using [packer.nvim](https://github.com/wbthomason/packer.nvim):

````bash
```lua
use { 'TSawyer87/tokyo_drift' }
````

## Usage

After installation, add this to your `init.vim` or `init.lua` if you didn't go
with the first option:

```bash
vim.cmd('colorscheme tokyo_drift')
```
