# sef (Shortcut Every File)

A quick bash script to run a command on target file extensions.

## Inspiration

Every once in a while, I want to quickly look at a file in command line. However, I have so many different terminal applications for different file extensions that I often forget the right command. Thus, `sef` was born. `sef` is a quick bash script to run a preset command on a file from command line.

### But what about `xdg-open`?!

I don't always want to use my default program on a specific file. `sef` serves as a secondary layer of commands that I can easily run on any file extension.

For example, `xdg-open README.md` will open `README.md` in vim, but what I really want to do is open it in [glow](https://github.com/charmbracelet/glow).

## Usage

`sef README.md`

This will run whatever command you set for `*.md` on `README.md`.

## Install

- Copy `sef` to `./local/bin`
- Ensure that `./local/bin` in your `$PATH`
- Create a config file `sef.conf` at `$XDG_CONFIG_HOME/sef`

### `senf.conf` format

The format of the config file is the following:

`command ext1,ext2,ext3`


## Todo

- Add extension command to avoid manually editing the config file (using `sed`?)
- Support for flags
- List extension command
- Search extension command
