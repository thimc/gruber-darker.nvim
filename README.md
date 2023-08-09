# gruber-darker.nvim

Gruber darker theme for Neovim written entirely in lua.

Based on [Alexey's version of the gruber darker theme](https://github.com/rexim/gruber-darker-theme).

![Screenshot. with transparent true](https://github.com/thimc/gruber-darker.nvim/blob/main/screenshot.png)

## Installation

<details>
<summary>Expand packer snippet: </summary>

```lua
return require('packer').startup(function(use)
  use {'wbthomason/packer.nvim'}

  use {'thimc/gruber-darker.nvim'}
end)
```
</details>

<details>
<summary>Expand lazy snippet: </summary>

```lua
{
  'thimc/gruber-darker.nvim',
  config = function()
    require('gruber-darker').setup({
      -- OPTIONAL
      transparent = true, -- removes the background
      -- underline = false, -- disables underline fonts
      -- bold = false, -- disables bold fonts
    })
    vim.cmd.colorscheme('gruber-darker')
  end,
}
```
</details>

## Supported plugins

I don't use all that many plugins, instead I rely on the built in commands
such as netrw, vimdiff and spellcheck. So I haven't really extended the themes
support but I can confirm that popular plugins such as treesitter, telescope
and fugitive work fine.


Pull requests are more than welcome!
