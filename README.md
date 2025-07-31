# dotfiles

Using [chezmoi](https://www.chezmoi.io) for management.

Tips:

```sh
# Pull changes on disk into chezmoi
chezmoi re-add
```

## Setup

Install git and setup ssh.

```sh
winget install --id Git.Git -e --source winget

ssh-keygen -t ed25519 -C "33764106+joshsj@users.noreply.github.com"

eval "$(ssh-agent -s)"

ssh-add ~/.ssh/id_ed25519

# add .pub to GH
# https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key
```

Install chezmoi and pull my dotfiles

```sh
winget install twpayne.chezmoi

chezmoi init git@github.com:joshsj/dotfiles

chezmoi apply -v
```

## Fonts

[Iosevka Term (nerd font)](https://www.nerdfonts.com/font-downloads)

## Neovim

Install [kickstart.nvim dependencies](https://github.com/nvim-lua/kickstart.nvim?tab=readme-ov-file#install-external-dependencies)

## Dotnet

### SDKs

Setup IIS in Windows features

Dotnet SDK(s): `winget install Microsoft.DotNet.SDK.8`

Dotnet dev certificate: `dotnet dev-certs https -t -q`

### IDE

Install [JetBrains Toolbox](https://www.jetbrains.com/toolbox-app)

Install Rider plus theme(s) and IdeaVim

