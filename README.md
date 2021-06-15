## Setup dotfiles on a new machine

1. Install chezmoi to `~/.local/bin`.
   ```
   $ BINDIR=$HOME/.local/bin curl -sfL https://git.io/chezmoi | sh
   ```
1. Initialize chezmoi.
   ```
   $ bin/chezmoi init https://github.com/tbonfort/dotfiles.git
   ```
1. (Optional) Check the diff.
   ```
   $ chezmoi apply -nv
   ```
1. Install the dotfiles.
   ```
   $ chezmoi apply
   ```

Done! To keep up to date in the future:

```
$ chezmoi update
```


