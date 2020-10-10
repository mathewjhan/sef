# sef (Shortcut Every File)

## Inspiration

Every once in a while, I want to quickly look at a file in command line. However, I have so many different terminal applications for different file extensions that I often forget the right command. Thus, `sef` was born. `sef` is a quick bash script to run a preset command on a file from command line.

## But what about `xdg-open`?!

I don't always want to use my default program on a specific file. `sef` serves as a secondary layer of commands that I can easily run on any file extension.

## Install

- Copy `sef` to `./local/bin`
- Ensure that `./local/bin` in your `$PATH`
- Create a config file `sef.conf` at `$XDG_CONFIG_HOME/sef`

### Config format

The format of the config file is the following:

`command ext1,ext2,ext3`


## Todo

- Add extension command to avoid manually editing the config file (using `sed`?)
- List extension command
- Search extension command
