# dotfiles

## Install
⚠️ **Warning:** The `git checkout --force` command may overwrite files in your home directory.

```shell
export GIT_DIR=$HOME/repos/work/dotfiles
export GIT_WORK_TREE=$HOME

git clone --bare https://github.com/doughom/dotfiles $GIT_DIR
git config status.showUntrackedFiles no
git checkout --force
```
