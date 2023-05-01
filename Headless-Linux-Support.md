# **Only tested on Ubuntu for now.**

RustDesk 1.2 (nightly build)

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

# Alternative solutions
- Intel virtual display: https://github.com/rustdesk/rustdesk/issues/59#issuecomment-1494257375
- Fake / dummy hdmi https://github.com/rustdesk/rustdesk/issues/59#issuecomment-1494275098 https://github.com/rustdesk/rustdesk/issues/59#issuecomment-1162817430
- Configure dummy display yourself, https://github.com/rustdesk/rustdesk/issues/3592
