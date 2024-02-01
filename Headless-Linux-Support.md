
## Rustdesk supports Dummy Monitors on Xorg

Rustdesk has been [made compatible](https://github.com/rustdesk/rustdesk/pull/3902) and tested to work with the virtual Xorg driver [`xf86-video-dummy`](https://gitlab.freedesktop.org/xorg/driver/xf86-video-dummy) used to create dummy displays for headless server with graphical access.

It is now enabled automatically, so there is no setting to activate within Rustdesk. Simply install it normally on your system using X11 with `xf86-video-dummy` driver and a "dummy" monitor.

Linux Distributions successfully tested:
- **Ubuntu**
- **Arch Linux**

Desktop Environment/Window Managers sucessfully tested:
- **Gnome**
- **i3**

xfce4 may be supported.

Prerequirements:
```bash

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

#Create dummy monitor in Xorg config
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
