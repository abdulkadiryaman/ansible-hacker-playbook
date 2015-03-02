ansible-hacker-playbook
=======================

An [ansible](http://ansible.cc) playbook that sets up my development environment from scratch.

Features
--------

- Installs and sets up following technologies on Ubuntu 14.10

  - languages :
    - [Go 1.4.2](https://storage.googleapis.com/golang/go1.4.2.linux-amd64.tar.gz)
    - [Java8](ppa:webupd8team/java)
    - [Nodejs latest](https://deb.nodesource.com/setup)
    - python2.7
  - utilities:
    - [apt-fast](ppa:saiarcot895/myppa)
    - [unity network speed indicator](ppa:nilarimogard/webupd8)
    - tmux as default shell, and set zsh default in tmux
    - [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) with git plugin enabled
  - apps:
    - google chrome
  - vim.plugins
    - [molokai.vim](https://github.com/fatih/molokai.git)
    - [vim.go](https://github.com/fatih/vim-go.git)
    - [javascript](https://github.com/pangloss/vim-javascript.git)
    - [tagbar](https://github.com/majutsushi/tagbar.git)
    - [nerdtree](https://github.com/scrooloose/nerdtree.git)
    - [pathogen](https://tpo.pe/pathogen.vim)
    - [youcompleteme](https://github.com/Valloric/YouCompleteMe.git)
    - [conque-shell](https://github.com/eternnoir/Conque-Shell.git)
    - [solarized theme for gnome-terminal](git@github.com:Anthony25/gnome-terminal-colors-solarized.git)

Running
-------

- [install ansible on ubuntu](http://docs.ansible.com/intro_installation.html#latest-releases-via-apt-ubuntu)
- `sudo apt-get install openssh-server sshpass`
- `in tasks/shell.yml change the 5th line *user=abdulkadir* with your user on ubuntu`
- `ansible-playbook -i ubuntu --ask-pass --ask-sudo-pass site.yml`

Authors
-------
- Initial version: [Luke Macken](http://lewk.org) ([@lmacken](http://twitter.com/lmacken))

- Modified to apt-get: Abdulkadir Yaman ([@abdulkadiryaman](http://twitter.com/abdulkadiryaman)
