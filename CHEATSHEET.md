# NeoVim Commands + Cheat Sheat

## :Lexplore
(brings up simplfied file explorer)
(now replaced by (leader)E, which is <Space> + e

## :vsplit
(splits the screen vertically into 2)

## :splits
(splits horizontally)

`Ctrl-W k` becomes `Ctrl-k` (moves up one window)
`Ctrl-W j` becomes `Ctrl-j` (moves down one window)
`Ctrl-W k` becomes `Ctrl-h` (moves left one window)
`Ctrl-W k` becomes `Ctrl-l` (moves right one window)

## :resize -2<CR> becomes Ctrl-Up (pushes window bar up)
`:resize +2<CR>` becomes `Ctrl-Down` (pushes window bar down)
`:vertical resize -2<CR>` becomes `Ctrl-Left` (pushes window bar left)
`:vertical resize +2<CR>` becomes `Ctrl-Right` (pushes window bar right)


## :bnext
(goes to the next buffer)
(now replaced by L)
`:bprev`
(goes to the previous buffer)
(now replaced by H)

## Insert mode:
`jk` = exits mode

## Visual Mode:
`<` = move the code to the left
`>` = move the code to the right

`Alt+j` (moves selected text up)
`Alt+k` (moves selected text down)

## `:packer + <Tab>`
(all the packer commands to install plug-ins)

## `:colorscheme + <Tab>`
(change the color scheme)

## `:LspInstallInfo`
(shows you the LSP languages installed)

## `:LspInfo`
(info on the current language installed)

## Syntax Error Mode:
`gl` (more info about the error)

## <tab> and <return>:
(Just type the `function name + <Tab>` and the result is completion. Hit the `<enter>` to complete it. Works for functions, snippets,
and buffers.

## LSPInstallInfo
(just type `:LspInstallInfo + <Enter>` key. After that, you can search by typing `/` (forward slash) and then what you want to
search for. Type 'I' to install the server(s) you need)

## Telescope

Type this to search for files (with a preview box):
`Telescope find_files + <Enter> key`

To search for all your TODOs and anything involving text
`:Telescope live_grep + <Enter> key`

Type the following to go to the definition of a function
`:Telescope lsp_definitions + <Enter> key`

For a list of all definitions:
`gr` (on top of the name of a function)

Or:
`:Telescope lsp_definitions` (same as typing gd)

Here is another way:
`:Telescope lsp_references`

To display a quick fix list:
`gr`

To display Git branches:
`:Telescope git_branches`

To display your Git status:
`:Telescope git_status`

To display some git commits:
`:Telescope git_commits`

Searches for files at the bottom of the screen 
`:Telescope find_files theme=ivy`

For a more dropdown version:
`:Telescope find_files theme=dropdown`

## Comments

To comment a line out, type:
`gcc`

For multiple lines, type:
highlight the lines in visual mode, then type `gc`

## GitSigns

For a full list of commands:
`:GitSigns + <tab>`

## Nvim-tree
(all of these commands work within the actual tree and not the editor window

To move to left window:
`<Ctrl> + h`

to move to right window:
i`<Ctrl> + l`

To enter a file:
`<enter>`

NvimTreeToggle:
`<Spacebar> + e`

More command:
`:Nvim + <tab>`

From within a directory, to create a new file (and over the fileaname):
`a`

From within a directory, to rename a file (and over the fileaname):
`r`

From within a directory, to delete a file (and over the fileaname)
`d`

To close a directory / node:
`h`

To open a directory / node:
`l`

For a vertical split of the window:
`v`

## Bufferline
To switch buffers to the left:
`<Shift> + h`

To switch buffers to the right:
`<Shift> + l`

To switch buffers using letters:
`:BufferLinePick + <key>`

The buffers are clickable!

Starting a new tab:
`:tabnew %`

To move between tabs:
`gt`

To Close a buffer:
`:Bdelete`

To view highlights:
`:hi + <Tab>`

## Null-ls

When you have an error, for more information type:
`gl`

To format your file using LSP:
`:lua vim.lsp.buf.formatting_sync()`

`:lua vim.lsp.formatting_sync()`

## Toggleterm

To toggle Toggleterm:
`<Ctrl> + \`

To toggle LazyGit:
`:lua _LAZYGIT_TOGGLE`

## Whichkey

To comment a file:
`<spacebar> + /`

To call up the dashboard:
`<spacebar> + a`

To switch buffers / files:
`<spacebar> + b`

To toggle NvimTree / the file explorer:
`<spacebar> + e`

To save a file (i.e. much faster than :w):
`<spacebar> + w`

To quit Neovim (i.e. much faster than :q):
`<spacebar> + q`

To close a buffer / file:
`<spacebar> + c`

For no highlight:
`<spacebar> + h`

To find /search your files:
`<spacebar> + f`

To find / search for text within your files:
`<spacebar> + F`

To Telescope projects / find files within your projects:
`<spacebar> + P`
 
For Packer related stuff:
`<spacebar> + p`

For Git related stuff:  
`<spacebar> + g`

For LSP related stuff:
`<spacebar> + l`

For Telescope related stuff:
`<spacebar> + s`

For Terminal related stuff:
`<spacebar> + t`

To quit Lazygit wihtin NeoVim:
`:q`

## nvim-ts-autotag

Tags can be automatically closed. For example:
`<html>` automatically results to: `<html></html>`

## NvimTreeToggle Extras

There are now 3 (i.e. not 2 as stated on the commit) added shortcuts when you type <Ctrl> + E:

1. `<Spacebar> + Q` to "Save and Quit"
2. `<Spacebar> + ec` to "Edit the config file (i.e. init.lua)"
