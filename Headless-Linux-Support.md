# **Only tested on Ubuntu for now.**

Prerequirements:
```bash
# Only support gnome desktop. https://www.gnome.org
# xfce4 may be supported.

# for Ubuntu
$ sudo apt install ubuntu-desktop
$ sudo apt install xserver-xorg-video-dummy
$ sudo apt install lightdm

# for Fedora
$ sudo sudo yum groups install "GNOME"
$ sudo yum install xorg-x11-drv-dummy

# for archlinux
$ pacman -S xorg xorg-server xf86-video-dummy
$ pacman -S gnome

```

Steps
```
# install rustdesk
# get rustdesk id
$ sudo rustdesk --get-id
# set password
$ sudo rustdesk --password <password>

# connect
```

TODOs:
- [ ] Do not show "Connection Error" on logout.

https://github.com/rustdesk/rustdesk/pull/3902#issue-1651369085