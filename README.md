# dotfiles

My simple an useful dot files. The structure is based on repository [https://github.com/webpro/dotfiles](https://github.com/webpro/dotfiles).

## Requirements

* macos
* git

## Install

Clone this repository:

```bash
git clone https://github.com/thiagosf/dotfiles.git ~/.dotfiles
```

Add the code bellow at the end of the `~/.bash_profile` file (if you do not have this file, create an empty one):

```bash
DOTFILES_DIR="$HOME/.dotfiles"
for DOTFILE in "$DOTFILES_DIR"/system/.{env,alias,function,git-completion}; do
  [ -f "$DOTFILE" ] && . "$DOTFILE"
done
```

Enjoy! :rocket:
