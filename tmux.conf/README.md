# tmux settings

## For local machine

Copy `.tmux.conf` file to your home directory

## For remote machine

1. Copy `.tmux.remote.conf` to your home directory of remote machine and rename it to `.tmux.conf`

2. Setup shell of your remote machine

### Bash
Add following lines to `~/.bashrc`

```sh
[[ $SSH_AUTH_SOCK != $HOME/.ssh/sock && -S $SSH_AUTH_SOCK ]] \
    && ln -snf "$SSH_AUTH_SOCK" "$HOME/.ssh/sock" \
    && export SSH_AUTH_SOCK="$HOME/.ssh/sock"
```

### Zsh

TBA

### Fish

TBA
