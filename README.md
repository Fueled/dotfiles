# Fueled's Dotfiles

[![Build Status](https://travis-ci.org/fueled/dotfiles.svg?branch=master)](https://travis-ci.org/fueled/dotfiles)

This is a base collection of dotfiles and scripts we use for customizing our dev-setup at Fueled. See http://dotfiles.github.io/ for more details.

OS related setup scripts can be found in `setup` folder.

## Features

* Sane defaults for Mac
* Zsh
* Git
* vim

## Setup

If you are using Mac OSX, this repo includes a script to install dependencies in this [script](setup/setup_mac.sh).

This [script](setup/osx_defaults.sh) will help you add some defaults to your mac.

### Installing dotfiles

Once you have installed basics software and libraries, you can install the dotfiles, by cloning this repo into `~/dotfiles` and symlinking the files inside it to your home directory `~`. Symlinking helps keep all your dotfiles maintainable inside a git repo, while being functional at the same time.

```shell
cd ~ && git clone --recursive git@github.com:fueled/dotfiles.git && cd ~/dotfiles
# To create symbolic links in your home
sh bootstrap.sh  ## this will create the required symlinks
pip install -r requirements.pip  ## essential python packages needed
```

After this, go and edit your name & email in `.gitconfig.local` & `.cookiecutter.rc`

## Resources

You can watch the following repositories to pick up changes that you like:

- [Saurabh Kumar's dotfiles](https://github.com/theskumar/dotfiles)
- [Sanyam Khurana's dotfiles](https://github.com/CuriousLearner/dotfiles)

## License

The code is available under the [MIT license](LICENSE).
