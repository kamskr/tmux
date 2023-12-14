# TMUX
My tmux setup

install tmux and tmux plugins

```
brew install tmux
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

To start iterm with tmux ad this sript to `Send text at start`:

```
tmux ls && read tmux_session && tmux attach -t ${tmux_session:-default} || tmux attach || tmux 
```

Run source config: 

```
tmux source ~/.config/tmux/tmux.conf
```

Run Ctrl + b + I to install packages

## Tmux sessionizer

https://github.com/ThePrimeagen/.dotfiles/blob/master/bin/.local/scripts/tmux-sessionizer
https://github.com/jrmoulton/tmux-sessionizer

First install rust following instauctions: https://doc.rust-lang.org/cargo/getting-started/installation.html
Then run `cargo install tmux-sessionizer` to install CLI tool

then you can use tms command, but firest setup default path to search for repositories f.e.:

```
tms -p ~/Files
```


