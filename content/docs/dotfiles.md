---
title: Dotfiles
description: Dotfiles for my macOS setup powered by [rcm][1].
---
## Install Homebrew

Website: [https://brew.sh][2]

```bash
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Clone dotfiles to home root

```bash
  cd ~ && git clone ... && mv dotfiles .dotfiles
```

## Install packages and apps

```bash
  brew bundle --file=.dotfiles/homebrew/Brewfile
```

## Synchronize home directory using rcm

```bash
  rcup -v
```

## Add new rc files

```bash
  mkrc .zshrc ...
```

## Setup Neovim
```bash
  ln -s ~/.neovim ~/.config/nvim
```

[1]:	https://thoughtbot.github.io/rcm/rcm.7.html
[2]:	https://brew.sh