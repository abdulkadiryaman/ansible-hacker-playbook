ansible-hacker-playbook
=======================

An [ansible](http://ansible.cc) playbook that sets up a tricked-out [zsh](http://zsh.org) & [vim](http://vim.org) environment.

Features
--------

- Installs [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh), A community-driven framework for managing your zsh configuration.
- Installs [spf13-vim](http://vim.spf13.com), "The Ultimate Vim Distribution"
- Installs tmux as default shell, and set zsh default in tmuz

Running
-------

- `install ansible`
- `sudo apt-get install openssh-server sshpass`
- `ansible-playbook --inventory 'localhost,' --ask-pass --ask-sudo-pass playbook.yml`

Authors
-------
- Initial version: [Luke Macken](http://lewk.org) ([@lmacken](http://twitter.com/lmacken))

- Modified to apt-get: Abdulkadir Yaman ([@abdulkadiryaman](http://twitter.com/abdulkadiryaman)
