# Neovim Configuration

This is a modular, modern Neovim configuration designed for productivity, aesthetics, and ease of use. It uses [lazy.nvim](https://github.com/folke/lazy.nvim) for plugin management and is centered around the beautiful **onemonokai** theme.

## Features

- Fast startup and lazy loading of plugins
- Clean, maintainable Lua code structure
- Pre-configured keymaps for efficient navigation and editing
- Modern UI with [onemonokai](https://github.com/bryanwills/one_monokai.nvim) theme

## Installation

1. **Clone this repository** into your Neovim config directory:
   ```sh
   git clone https://github.com/bryanwills/nvim ~/.config/nvim
   ```
2. **Open Neovim** and plugins will be installed automatically via `lazy.nvim`.
3. **Font Recommendation:** Use a Nerd Font (e.g., [MesloLGS Nerd Font](https://www.nerdfonts.com/)) for best icon support.

## Main Plugins

- [plenary.nvim](https://github.com/nvim-lua/plenary.nvim): Lua functions used by many plugins
- [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator): Seamless navigation between tmux and Vim splits
- [one_monokai.nvim](https://github.com/bryanwills/one_monokai.nvim): The main colorscheme/theme

## Theme

This config uses **onemonokai** as the only theme. All previous theme logic (e.g., tokyonight) has been removed for simplicity and consistency.

## Custom Keyboard Shortcuts

Below is a quick reference for the custom keymaps defined in this config. The `<leader>` key is set to the spacebar (`<Space>`).

| Mode | Shortcut     | Action              | Description                    |
| ---- | ------------ | ------------------- | ------------------------------ |
| i    | jk           | `<ESC>`             | Exit insert mode with jk       |
| n    | `<leader>nh` | `:nohl<CR>`         | Clear search highlights        |
| n    | `<leader>+`  | `<C-a>`             | Increment number               |
| n    | `<leader>-`  | `<C-x>`             | Decrement number               |
| n    | `<leader>sv` | `<C-w>v`            | Split window vertically        |
| n    | `<leader>sh` | `<C-w>s`            | Split window horizontally      |
| n    | `<leader>se` | `<C-w>=`            | Make splits equal size         |
| n    | `<leader>sx` | `<cmd>close<CR>`    | Close current split window     |
| n    | `<leader>to` | `<cmd>tabnew<CR>`   | Open new tab                   |
| n    | `<leader>tx` | `<cmd>tabclose<CR>` | Close current tab              |
| n    | `<leader>tn` | `<cmd>tabn<CR>`     | Go to next tab                 |
| n    | `<leader>tp` | `<cmd>tabp<CR>`     | Go to previous tab             |
| n    | `<leader>tf` | `<cmd>tabnew %<CR>` | Open current buffer in new tab |

- **Modes:** `n` = normal, `i` = insert
- `<leader>` = spacebar

## Customization

Feel free to edit the `lua/bryan/core/keymaps.lua` file to add or change keymaps to your liking.

---

Enjoy your new Neovim setup! For questions org suggestions, open an issue or PR on the repo.

