ubuntu-quick-config
===================

Quickly configures a fresh install of [Ubuntu 14.04 64-bit][tt] on a workstation or server.

*(The server part is a work in progress...)*

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [What it can do](#what-it-can-do)
- [Usage](#usage)
  - [Clone or download this project](#clone-or-download-this-project)
  - [Run it](#run-it)
- [SSH Keys](#ssh-keys)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## What it can do

- update [Ubuntu][ubuntu] and install some packages
- configure [git][git] global settings
- generate an [RSA key][sshkey] for remote [SSH sessions][ssh] (this is not a [GPG key][gpgkey])
- add useful [shell aliases][sa]
- make the [terminal][lc] easier to read and use
- add some plugins and a color scheme to [VIM][vim]
- add a color scheme to [gedit][gedit]
- install the latest [VirtualBox][vb], [Vagrant][vg] and setup [VVV][vvv] and [VV][vv] for [WordPress][wp] development

## Usage

### Clone or download this project

- HTTPS: `git clone https://github.com/keegoid/ubuntu-quick-config.git`
- SSH: `git clone git@github.com:keegoid/ubuntu-quick-config.git`

### Run it

Run the main program with `./run.sh`

If it doesn't work, you might need to do this:

```bash
chmod +x run.sh
dos2unix -k run.sh
```

Also run `./sudoers.sh` if you want to increase the sudo timeout which is set to 15 minutes by default.

## SSH Keys

You can save a backup copy of your [SSH key pair][sshkey] that gets generated and output to the screen. I prefer saving it as a secure note in [LastPass][lp]. Copy the keys from the [Linux console][lc] with `ctrl+shift+c` before clearing the screen.

```bash
cat ~/.ssh/id_rsa.pub
cat ~/.ssh/id_rsa
clear
```

## License

SEE: http://keegoid.mit-license.org


[ubuntu]:   http://www.ubuntu.com/global
[gedit]:    https://wiki.gnome.org/Apps/Gedit
[vim]:      http://www.vim.org/
[tt]:       https://wiki.ubuntu.com/TrustyTahr/ReleaseNotes
[lc]:       http://en.wikipedia.org/wiki/Linux_console
[vb]:       https://www.virtualbox.org/
[vg]:       https://www.vagrantup.com/
[vvv]:      https://github.com/Varying-Vagrant-Vagrants/VVV
[vv]:       https://github.com/bradp/vv
[wp]:       https://wordpress.org/
[ss]:       http://en.wikipedia.org/wiki/Shell_script
[ssh]:      http://en.wikipedia.org/wiki/Secure_Shell
[sshkey]:   http://en.wikipedia.org/wiki/Ssh-keygen
[gpgkey]:   http://en.wikipedia.org/wiki/GNU_Privacy_Guard
[sa]:       http://en.wikipedia.org/wiki/Alias_%28command%29
[gh]:       https://github.com/
[git]:      https://git-scm.com/
[lp]:       https://lastpass.com/f?3202156
[twitter]:  https://twitter.com/intent/tweet?screen_name=keegoid&text=loving%20your%20CentOS%207.0%20deploy%20scripts%20for%20%40middlemanapp%20or%20%40WordPress%20with%20%40nginxorg%20https%3A%2F%2Fgithub.com%2Fkeegoid%2Flinux-deploy-scripts
