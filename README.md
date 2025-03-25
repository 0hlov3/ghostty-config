# ghostty-config

Personal configuration files for the [Ghostty terminal emulator](https://ghostty.org/), managed with Git for easy synchronization across multiple machines.

## Install the Configuration

Clone this repository into your `~/.config` directory (or wherever your `XDG_CONFIG_HOME` points to):

### SSH

```shell
git clone git@github.com:0hlov3/ghostty-config.git "${XDG_CONFIG_HOME:-$HOME/.config}"/ghostty
```

### HTTPS

```shell
git clone https://github.com/0hlov3/ghostty-config.git "${XDG_CONFIG_HOME:-$HOME/.config}"/ghostty
```

## Usage
After cloning, Ghostty should automatically pick up the config if it’s in the correct directory:

```shell
# Expected config path:
$HOME/.config/ghostty/
```

Make any customizations you like, and push them back to keep your changes synced.

## Syncing Updates
When you make changes to your config on one machine:

```shell
cd "${XDG_CONFIG_HOME:-$HOME/.config}/ghostty"
git add .
git commit -m "Update config"
git push
```

Then, on another machine:

```shell
cd "${XDG_CONFIG_HOME:-$HOME/.config}/ghostty"
git pull
```

## About

This repo is tailored to my preferences, but feel free to fork it or use it as a base for your own setup!
