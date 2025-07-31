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
```

Install chezmoi and pull my dotfiles

```sh
winget install twpayne.chezmoi

chezmoi init git@github.com:joshsj/dotfiles

chezmoi apply -v
```

## .NET

```sh
winget install Microsoft.DotNet.SDK.8
```

Setup IIS in Windows features

Install [JetBrains Toolbox](https://www.jetbrains.com/toolbox-app) then whatever's needed

