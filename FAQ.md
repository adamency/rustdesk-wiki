# How does RustDesk work?
https://github.com/rustdesk/rustdesk/wiki/How-does-RustDesk-work%3F

# How much does the community version of RustDesk server cost? 
The community releases are free of charge if you wish to self host, no license is required. 
# Can I host my own RustDesk server? 
- Yes, you can host your own RustDesk server 
- There's a guide here: https://rustdesk.com/docs/en/self-host/ 
# Where can I download RustDesk Server?
You can download RustDesk server from: 
- https://github.com/rustdesk/rustdesk-server
- [Docker Hub](https://registry.hub.docker.com/u/rustdesk)

# The server is asking me for a license, where can I get one from? 
Please ensure you have downloaded the newest release of RustDesk server as licenses are no longer required for the community release.

Some users reported they could not pull latest RustDesk server with docker in some countries.
https://github.com/rustdesk/rustdesk-server/issues/184

# Config client for self-hosting
https://rustdesk.com/docs/en/self-host/client/

https://rustdesk.com/docs/en/self-host/hardcode-settings/

# What does the server do, why do I need it? 
- It is primarily used to help your RustDesk clients to find each other. 
- Once this is done, it helps you try and get a direct connection between them. 
- If this fails and your client and controlled devices cannot talk directly to each other, the relay part of side the server will be used to handle the connection. 
# I only use RustDesk for a few devices on my local network with no Internet connectivity... Can I still use RustDesk with direct ip access? 
Yes, you can! 

By default this is turned off for security, however if wish to allow this you can do so by doing steps below: 
- On the device you wish to control 
- Go into the Menu and select Enable direct IP...  
- On the client you are connecting from you can now input the Local IP address or host name the address box and click connect. 
- the connection is unecrypted, please do not send us issue about this.

# hbbs -c,  the configuration file format
Supper simple format just a=b on each line, a is the name of the option you see from the --help. e.g.
e.g.
```
port=123456
```

You can also put them in .env file under the same directory of hbbs/hbbr. hbbs/hbbr reads .env file no matter if you specify -c. 
![image](https://user-images.githubusercontent.com/71636191/173327939-4ed089cc-81bc-416a-a22e-6abc2791cfc4.png)

# Web client

https://rustdesk.com/docs/en/dev/build/web/

http://web.rustdesk.com/ no https for the time being

# Change id, addressbook/api/login and web console?

https://github.com/rustdesk/rustdesk-server/issues/22

https://github.com/rustdesk/rustdesk/discussions/570

https://github.com/rustdesk/rustdesk/issues/509 

# Hardware requirement for RustDesk server.
The hardware requirements are very low, the minimum configuration of the cloud server is enough, and the CPU and memory requirements are the minimum. Regarding the network size, if the TCP hole punching direct connection fails, the relay traffic will be consumed. The traffic of a relay connection is between 30k-3M/s (1920x1080 screen), depending on the resolution settings and screen update. If it is only for office work demand, the traffic is around 100K/s. 

# Deploy RustDesk server in intranet.
If you host the server in your intranet with some type of routers, you may have network problem because of NAT hairping,

https://www.reddit.com/r/rustdesk/comments/13fkdyd/comment/jjvm6j1/?utm_source=share&utm_medium=web2x&context=3

https://github.com/rustdesk/rustdesk-server/issues/24#issuecomment-1234029480

https://github.com/rustdesk/rustdesk/issues/732#issuecomment-1300514997

https://github.com/rustdesk/rustdesk/issues/732#issuecomment-1319433120

https://www.reddit.com/r/rustdesk/comments/1174mgw/comment/j9e9avt/?context=3

https://github.com/rustdesk/rustdesk-server/issues/200#issuecomment-1543710510

https://github.com/rustdesk/rustdesk-server/issues/134#issuecomment-1303437173

# X11 error: connection refused (login as root)

https://github.com/rustdesk/rustdesk/issues/2573#issuecomment-1408672281

# How to update RustDesk server?

https://github.com/techahold/rustdeskinstall/issues/30

# Some RustDesk Server installer
https://github.com/techahold/rustdeskinstall

https://github.com/elico/rustdesk-ansible-installer

# About self-hosting setup

- Most users can make it work following the tutorial: https://rustdesk.com/docs/en/self-host/install/
- This two videos should be helpful. https://www.youtube.com/watch?v=9nzHm3xGz2I and https://www.youtube.com/watch?v=EeFqj23jxMk. Another one in French: https://www.youtube.com/watch?v=J7t32K5--cM
- Most questions are about Linux and network, which can be Googled and ChatGPTed.
- Go to [Discord](https://discord.gg/nDceKgxnkV), there may be some nice users help you. Or search in the discord `welcome` channel, there are many users who have asked similar questions. Whenever, search is your best friend.
- If you host the server in your intranet with some type of routers, you may have network problem because of NAT hairping, 

>   - https://github.com/rustdesk/rustdesk-server/issues/24#issuecomment-1234029480 
>   - https://github.com/rustdesk/rustdesk/issues/732#issuecomment-1300514997 
>   - https://github.com/rustdesk/rustdesk/issues/732#issuecomment-1319433120

- With nginx: https://github.com/rustdesk/rustdesk/issues/835#issuecomment-1162169296
- arm https://github.com/rustdesk/rustdesk-server/issues/125#issuecomment-1320943098
- Change id, addressbook/api/login and web console? https://github.com/rustdesk/rustdesk/wiki/FAQ#change-id-addressbookapilogin-and-web-console
- Windows
  - https://github.com/rustdesk/rustdesk/discussions/2152
  - https://pedja.supurovic.net/setting-up-self-hosted-rustdesk-server-on-windows/
  - https://www.reddit.com/r/rustdesk/comments/12g9jmi/installing_your_own_rustdesk_server_on_a_windows/
- firewalls https://www.reddit.com/r/rustdesk/comments/11u5aou/unable_to_connect_ubuntu_machine_to_selfhosted/

> **Again, the document is open source, modify it if you do not like it, https://github.com/rustdesk/doc.rustdesk.com**



<div align="left">
      <a href="https://www.youtube.com/watch?v=9nzHm3xGz2I">
         <img src="https://img.youtube.com/vi/9nzHm3xGz2I/0.jpg" style="width:100%;">
      </a>
</div>
<div align="left">
      <a href="https://www.youtube.com/watch?v=EeFqj23jxMk">
         <img src="https://img.youtube.com/vi/EeFqj23jxMk/0.jpg" style="width:100%;">
      </a>
</div>

<div align="left">
      <a href="https://www.youtube.com/watch?v=9nzHm3xGz2I">
         <img src="https://img.youtube.com/vi/9nzHm3xGz2I/0.jpg" style="width:100%;">
      </a>
</div>
<div align="left">
      <a href="https://www.youtube.com/watch?v=PDnqFnnbVHg">
         <img src="https://img.youtube.com/vi/PDnqFnnbVHg/0.jpg" style="width:100%;">
      </a>
</div>

# Connection log on server side.

https://github.com/rustdesk/rustdesk-server/blob/4d6d439b1ad797f8f8741a42672fa46c1503672e/src/rendezvous_server.rs#L608

You need to enable it via env `RUST_LOG=debug`, e.g.

```
RUST_LOG=debug ./hbbs ....
```

# How does it work?

https://github.com/rustdesk/rustdesk/wiki/How-does-RustDesk-work%3F

# Access Logs?

Mac: `~/Library/Logs/RustDesk/server/`

Linux: `/root/.local/share/logs/RustDesk/server/`

Windows: 
- Portable: `%AppData%\Roaming\RustDesk\log\server\`
- Installed: `C:\Windows\ServiceProfiles\LocalService\AppData\Roaming\RustDesk\log\server\`

# Wayland
Wayland is experimentally supported in nightly build (1.2), but with some limitations.

https://github.com/rustdesk/rustdesk/issues/4276#issuecomment-1537105758

# Change default options
![image](https://github.com/rustdesk/rustdesk/assets/71636191/68d1aa91-d59c-43ac-bd6e-dca6dbfe7c34)

# No sound
https://github.com/rustdesk/rustdesk/issues/4280#issuecomment-1543618744

# Sponsor open source RustDesk (Donate)
https://github.com/sponsors/rustdesk

https://ko-fi.com/rustdesk

# Why does self-hosting server need to configure a public key?

https://github.com/rustdesk/rustdesk/discussions/966#discussioncomment-6017364

# Hide connection popup

https://github.com/rustdesk/rustdesk/discussions/4424

# White screen on windows

https://github.com/rustdesk/rustdesk/issues/418#issuecomment-1595882547

# Nginx stream proxy

https://github.com/rustdesk/rustdesk-server/issues/265

# Managed vs unmanaged
https://www.reddit.com/r/rustdesk/comments/14y6u8c/looking_into_rustdesk_but_have_a_question/

# Keyboard translation modes

>  RustDesk >= 1.2.0

<img width="158" alt="image" src="https://github.com/rustdesk/rustdesk/assets/71636191/44cf2b80-de97-4ea3-ba1d-73acedb6c636">


- Map mode

With "Map 1:1", all keys are mapped from the local to the remote keyboard based on their position. For example, the key "q" on a local QWERTY keyboard will transmit an "a" character if connected to a remote device with an AZERTY keyboard.

This mode is not recommended for office work but it can be useful if the remote device uses specialty software to map macros to specific keys.


- Translate mode

When "Translate" is selected, all keys will be transmitted to the remote endpoint as if the local keyboard layout is active on the remote device.

However, this layout mode may cause problems with certain programs such as video games as they use scan code to process the key presses.

- Legacy mode

This mode is for compatibility with RustDesk <= 1.1.9.

# Force relay

>  RustDesk >= 1.2.0

Some users experience connection problems when using the desktop or mobile client, but not when using the web client. This is because the web client always uses a relay for connection. To resolve the issue, you can add the suffix '/r' to the remote ID.

<img width="295" alt="image" src="https://github.com/rustdesk/rustdesk/assets/71636191/98d601ea-f84a-447e-a93b-f48a07850796">

or 

![image](https://github.com/rustdesk/rustdesk/assets/71636191/e5df3d73-6656-43ad-ba7e-557e7a4873ed)

# Headless Linux Support

https://github.com/rustdesk/rustdesk/wiki/Headless-Linux-Support

