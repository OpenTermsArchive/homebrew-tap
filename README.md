# Open Terms Archive Homebrew Tap

[Homebrew](https://brew.sh/) is a package manager to install, update, and manage software on macOS. This repository is a custom [tap](https://docs.brew.sh/Formula-Cookbook#page), that means it's a directory of formulae that lets install software from outside the main Homebrew repositories.

Homebrew's core repository only keeps the latest version of each package, which is why this repository makes available specific versions of the software used on different Open Terms Archive projects.

## Install

`brew tap OpenTermsArchive/homebrew-tap https://github.com/OpenTermsArchive/homebrew-tap`

## Uninstall

`brew untap OpenTermsArchive/homebrew-tap`

## Update

`cd "$(brew --repo OpenTermsArchive/homebrew-tap)" && git pull`

## Install a formula

`brew install <formula>@<version>`

## Uninstall a formula

`brew uninstall <formula>@<version>`

## Switch of version

1. `brew unlink <formula>@<version>`
2. `brew link <formula>@<version>`

## Hugo versions

Learn [how to add a Hugo formula](./how-to-add-hugo-formula.md).
