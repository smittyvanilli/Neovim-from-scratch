# NeoVim Commands + Cheat Sheat

## :Lexplore
(brings up simplfied file explorer)
(now replaced by (leader)E, which is <Space>+e

## :vsplit
(splits the screen vertically into 2)

## :splits
(splits horizontally)

Ctrl-W k becomes Ctrl-k (moves up one window)
Ctrl-W j becomes Ctrl-j (moves down one window)
Ctrl-W k becomes Ctrl-h (moves left one window)
Ctrl-W k becomes Ctrl-l (moves right one window)

## :resize -2<CR> becomes Ctrl-Up (pushes window bar up)
:resize +2<CR> becomes Ctrl-Down (pushes window bar down)
:vertical resize -2<CR> becomes Ctrl-Left (pushes window bar left)
:vertical resize +2<CR> becomes Ctrl-Right (pushes window bar right)


## :bnext
(goes to the next buffer)
(now replaced by L)
:bprev
(goes to the previous buffer)
(now replaced by H)

## Insert mode:
jk = exits mode

## Visual Mode:
< = move the code to the left
> = move the code to the right

Alt+j (moves selected text up)
Alt+k (moves selected text down)

## :packer+<Tab>
(all the packer commands to install plug-ins)

## :colorscheme+<Tab>
(change the color scheme)

## :LspInstallInfo
(shows you the LSP languages installed)

## :LspInfo
(info on the current language installed)

## Syntax Error Mode:
gl (more info about the error)

## <tab> and <return>:
(Just type a function + <Tab> and the result is completion. Hit the <enter> to complete it. Works for functions, snippets,
and buffers.

## LSPInstallInfo
(just type :LspInstallInfo + <Enter> key. After that, you can search by typing '/' (forward slash) and then what you want to
search for. Type 'I' to install the server(s) you need)
