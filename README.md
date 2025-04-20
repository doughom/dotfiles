# dotfiles

## Install
⚠️ **Warning:** The `git checkout --force` command may overwrite files in your home directory.

Linux/macOS:
```shell
export GIT_DIR=$HOME/repos/work/dotfiles
export GIT_WORK_TREE=$HOME

git clone --bare https://github.com/doughom/dotfiles $GIT_DIR
git config status.showUntrackedFiles no
git checkout --force
```

Windows:
```powershell
$env:GIT_DIR="$env:USERPROFILE/repos/work/dotfiles"
$env:GIT_WORK_TREE=$env:USERPROFILE

git clone --bare https://github.com/doughom/dotfiles $env:GIT_DIR
git config status.showUntrackedFiles no
git checkout --force
```

## Setup Conditional Includes
Create separate `.gitconfig` files for each account:

```
[credential "https://github.com"]
    username = githubusername
[user]
    name = Name
    email = 123456789+githubusername@users.noreply.github.com
```