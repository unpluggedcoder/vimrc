# vimrc

Install all vim plugs with `:PlugInstall`.

## Rust

I use [`coc-rls`](https://github.com/neoclide/coc-rls) instead `rust-lang/rls` vim plug, so do the `rust-analyzer`.
Install Coc extensions with below:

```shell
:CocInstall coc-rls
:CocInstall coc-rust-analyzer
```

You should have `rust-analyzer` binary in your `$PATH`, or just set the executable path for `dense-analysis/ale`.

# tmux

## Installation

Requirements: tmux version 1.9 (or higher), git, bash.

Clone TPM:

```shell
$ git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

Copy `.tmux.conf` to `~/.tmux.conf` ($XDG_CONFIG_HOME/tmux/tmux.conf works too).

### Installing plugins

1. Add new plugin to `~/.tmux.conf` with `set -g @plugin '...'`
2. Press `prefix` + <kbd>I</kbd> (capital i, as in **I**nstall) to fetch the plugin.

You're good to go! The plugin was cloned to `~/.tmux/plugins/` dir and sourced.

### Uninstalling plugins

1. Remove (or comment out) plugin from the list.
2. Press `prefix` + <kbd>alt</kbd> + <kbd>u</kbd> (lowercase u as in **u**ninstall) to remove the plugin.

All the plugins are installed to `~/.tmux/plugins/` so alternatively you can
find plugin directory there and remove it.

