---
title: dotfiles
draft: false
---

Portable personalization of my development environments. Updates are extremely stochastic, based on when I get new boxen. Suitability to any other environment is not assumed or desired.

[Github](https://github.com/gaylatea/dotfiles)

# Prior art
* [Mathias Bynen](https://github.com/mathiasbynens/dotfiles)
* [`chezmoi`](https://www.chezmoi.io/)
  * [Tom Payne's own dotfiles](https://github.com/twpayne/dotfiles)

# Ease of use

## One-liner
Similar to [Homebrew](https://brew.sh), I wanted a one-line install command that I could run on a new machine and have it automatically do the needful for me.

The install script will load Homebrew/oh-my-zsh, install all my `Brewfile` dependencies, and then symlink any config files I use from the repo into their correct places. It also installs an alias, `dotsync`, that I can use to sync my changes from other machines.

## Secrets
When I run the install script, it will prompt me for the password to my `age` key. Using this key, I can encrypt any sensitive files in the repo, and decrypt/symlink them locally.

# macOS
I've largely cargo-culted settings from [Mathias' dotfiles](https://github.com/mathiasbynens/dotfiles/blob/main/.macos), which streamline a lot of the macOS settings. I plan on auditing this a little more.
