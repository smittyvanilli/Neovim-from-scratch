# Neovim from scratch

My NeoVim config is inspired by the NeoVim From Scratch YouTube series.

Color scheme has been changed to default for VSCode / VSCodium.

Completions have been added.

More color scheme has been added by treesiter plug-in

Added abilities for faster comments.

Added the ability for Git signs.

Add NVim-Tree, an improved file explorer. Disclaimer: there were lots of fixes I had to do to get his working!

Add buffers / tabs, like in VSCode / Atom. 

Add ability to lint / error-check your files using external methods and LSP.

New and improved status line at the bottom.

Added a floating terminal plugin

Added impaient plugin. Load times will be faster.

Lines will be indented in source files from the indentline plugin.

The following is copied from Christian Chiarulli's README file.
(https://github.com/LunarVim/Neovim-from-scratch/blob/master/README.md)

---

**Important Update** When I initially created this repo I didn't anticipate the amount of breaking changes, if you'd like to use the same basic config as this one as a base I recommend my new repo: [nvim-basic-ide](https://github.com/LunarVim/nvim-basic-ide)

**Another Update** This repo should work fine with Neovim 0.8, also all packages are pinned so it should remain stable.

Each video will be associated with a branch so checkout the one you are interested in, you can follow along with this [playlist](https://www.youtube.com/watch?v=ctH-a-1eUME&list=PLhoH5vyxr6Qq41NFL4GvhFp-WLd5xzIzZ).

## Try out this config

Make sure to remove or move your current `nvim` directory

**IMPORTANT** Requires [Neovim v0.8.0]](https://github.com/neovim/neovim/releases).  [Upgrade](#upgrade-to-latest-release) if you're on an earlier version. 
```
git clone https://github.com/LunarVim/Neovim-from-scratch.git ~/.config/nvim
```

Run `nvim` and wait for the plugins to be installed 

**NOTE** (You will notice treesitter pulling in a bunch of parsers the next time you open Neovim) 

## Get healthy

Open `nvim` and enter the following:

```
:checkhealth
```

You'll probably notice you don't have support for copy/paste also that python and node haven't been setup

So let's fix that

First we'll fix copy/paste

- On mac `pbcopy` should be builtin

- On Ubuntu

  ```
  sudo apt install xsel
  ```

- On Arch Linux

  ```
  sudo pacman -S xsel
  ```

Next we need to install python support (node is optional)

- Neovim python support

  ```
  pip install pynvim
  ```

- Neovim node support

  ```
  npm i -g neovim
  ```
---

**NOTE** make sure you have [node](https://nodejs.org/en/) installed, I recommend a node manager like [fnm](https://github.com/Schniz/fnm).

### Upgrade to latest release

Assuming you [built from source](https://github.com/neovim/neovim/wiki/Building-Neovim#quick-start), `cd` into the folder where you cloned `neovim` and run the following commands. 
```
git pull
make distclean && make CMAKE_BUILD_TYPE=Release
sudo make install
nvim -v
```

> The computing scientist's main challenge is not to get confused by the complexities of his own making. 

\- Edsger W. Dijkstra
