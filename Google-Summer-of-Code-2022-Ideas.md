RustDesk project would like to participate in Google Summer of Code 2022.

https://github.com/rustdesk/rustdesk/wiki/Google-Summer-of-Code-2021

## Project Ideas

### Wayland Support

Skills: Rust, C/C++, Linux

Description:
RustDesk support X11 on Linux, but does not support Wayland yet. Wayland has totally different API for screen capture and keyboard/mouse input compared with X11. Wayland has strict permission control, you can only capture screen under the user session. A permission dialog will pop up once you initiates screen capture, this causes big problem for remote control scenario.

Resources:
 - Discuss on Wayland support: https://github.com/rustdesk/rustdesk/issues/56
 - Initial job done for Wayland, only screen capture: https://github.com/rustdesk/rustdesk/tree/master/libs/scrap/src/wayland

