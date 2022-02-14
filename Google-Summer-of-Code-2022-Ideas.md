RustDesk project would like to participate in Google Summer of Code 2022.

https://github.com/rustdesk/rustdesk/wiki/Google-Summer-of-Code-2022

## Project Ideas

### Wayland Support

Skills: Rust, C/C++, Linux

Description:
RustDesk support X11 on Linux, but does not support Wayland yet. Wayland has totally different API for screen capturing and keyboard/mouse input. Wayland has strict permission control, you can only capture screen under the user session. A permission dialog will pop up once you initiates screen capturing, this causes big problem for remote control scenario.

Resources:
 - Discuss on Wayland support: https://github.com/rustdesk/rustdesk/issues/56
 - Initial job done for Wayland, only screen capturing: https://github.com/rustdesk/rustdesk/tree/master/libs/scrap/src/wayland

### Migrate UI from Sciter to Tauri

Skills: Rust, Javascript

Description:
RustDesk chose Sciter as its Desktop UI SDK. As Tauri turns to be stable, it is time to switch to a more elegant UI SDK. Current RustDesk UI is based on TIScript+html+css, TIScript is a modified version of Javascript. After migration, RustDesk will switch to multiple windows mode to have better OS taskbar integration.

Resources:
 - Tauri project: https://github.com/tauri-apps/tauri
 - What is Sciter?: https://sciter.com/
 - Multiple windows issue: https://github.com/rustdesk/rustdesk/issues/293

### Whiteboard

Skills: Rust, Windows/Linux/Mac

Description: Whiteboard is additional collaboration tool while sharing desktop, which enables users write or draw freely on computer screen during presentations.

Resources:
 - Whiteboard in AnyDesk: https://anydesk.com/uk/features/whiteboard


### Recoverable file transfer

Skills: Rust, Javascript

Description: Current file transfer stops after disconnection or window being closed. This new feature make file transfer jobs can be manually paused and recoverable.

Resources:
 - Related issue: https://github.com/rustdesk/rustdesk/issues/358

