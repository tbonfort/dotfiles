## Setup dotfiles on a new machine
```bash
   export BINDIR=$HOME/.local/bin
   export PATH=$PATH:$BINDIR
   curl -sfL https://git.io/chezmoi | sh
   chezmoi init https://github.com/tbonfort/dotfiles.git
   chezmoi apply
   source $HOME/.bashrc
```

Done! To keep up to date in the future:

```
$ chezmoi update
```


