# Neovim
---
"the cult of vi vs the church of emacs"

vim tutorial and commands -> [[VIM]]


__guides__:
- [[nvim + vimtex + zathura]]

__plugins__:
- [packer.nvim](https://github.com/wbthomason/packer.nvim)
- [alpha-nvim](https://github.com/goolord/alpha-nvim)
- [auto-save.nvim](https://github.com/Pocco81/auto-save.nvim)
- [true-zen.nvim](https://github.com/Pocco81/true-zen.nvim)
- [twilight.nvim](https://github.com/folke/twilight.nvim)





---
edit or delete
[neovim lua documentation](https://neovim.io/doc/user/lua.html)
[neovim options documentation](https://neovim.io/doc/user/options.html)
[lua main page](https://www.lua.org/home.html)
[lua reference manual](https://www.lua.org/manual/5.4/)



https://medium.com/geekculture/neovim-configuration-for-beginners-b2116dbbde84
https://github.com/jdhao/nvim-config
https://www.youtube.com/results?search_query=neovim+lua+config
https://www.youtube.com/watch?v=_evGrg4l3CY
https://www.youtube.com/watch?v=36o52-2_83M
https://www.youtube.com/watch?v=qb6fPgZMRF4
https://www.youtube.com/watch?v=m62UCkdQ8Ck

https://www.youtube.com/watch?v=cAfPmPjxRQE
https://www.youtube.com/watch?v=Ku-m7eEbWas
https://www.youtube.com/watch?v=gccGjwTZA7k
https://www.youtube.com/watch?v=ctH-a-1eUME
---

]]

package management
packer -> install nvim-packer-git (aur)
then we can run :PackerSync

source with -> :so %
open up other files with -> e ~/(path)

enter a mentioned lua file with ctrl+o

you can access files (if the path is writen) with -> g + f
then go back to with -> ctrl + o

splitting the terminal
> :split -> duplicate and split the editor horizontally
> :vsp -> duplicate and split the editor vertically

move between them using
ctrl + w + h ->
ctrl + w + j ->
ctrl + w + k ->
ctrl + w + l ->


setting the

`g + f` -> enter the .lua file
`ctrl + o` -> go back to the original fileY



**vimtex**

#### Videos



install neovim
python modules -> python-pynvim

https://medium.com/geekculture/neovim-configuration-for-beginners-b2116dbbde84

---


 KEYBINDINGS
  2 -- vim.api.nvim_set_keymap({mode}, {keymap}, {mapped to}, {options})
  1 -- you can alias it to an easier to use -> local keymap = vim.api.nvim_set_keymap
  0 -- EXAMPLE: keymap('n', '<c-s>', ':w<CR>', {})
  1 -- you can also alias other -> local opts = { noremap = true }
  2 -- EXAMPLE: keymap('n', '<c-j>;, '<c-w>', opts)


# Themes or Configs

### [Neovim IDE / Vi Sual Studio Code](https://github.com/daniilty/vsnvim)

---
install nodejs gopls llvm (clang?)

git clone https://github.com/daniilty/vsnvim


**vimtex**

