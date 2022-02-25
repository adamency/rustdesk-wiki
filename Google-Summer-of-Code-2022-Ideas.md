RustDesk project would like to participate in Google Summer of Code 2022.

https://github.com/rustdesk/rustdesk/wiki/Google-Summer-of-Code-2022

## Project Ideas

### Wayland Support

Skills: Rust, C/C++, Linux

Description:
RustDesk support X11 on Linux, but does not support Wayland yet. Wayland has totally different API for screen capturing and keyboard/mouse input. Wayland has strict permission control, you can only capture screen under the user session. A permission dialog will pop up once you initiates screen capturing, this causes big problem for remote control scenario.

Outcome: RustDesk screen capturing and input control can work on Wayland.

Resources:
 - Discuss on Wayland support: https://github.com/rustdesk/rustdesk/issues/56
 - Initial job done for Wayland, only screen capturing: https://github.com/rustdesk/rustdesk/tree/master/libs/scrap/src/wayland

Rating: Hard

Size: 350 hours

Mentor: [Carrie Chow](https://github.com/rustdesk) RustDesk author

### Migrate UI from Sciter to Tauri

Skills: Rust, Javascript

Description:
RustDesk chose Sciter as its Desktop UI SDK. As Tauri turns to be stable, it is time to switch to a more elegant UI SDK. Current RustDesk UI is based on TIScript+html+css, TIScript is a modified version of Javascript. After migration, RustDesk will switch to multiple windows mode with tab window support to have better OS taskbar integration. Each connection keeps UI and logic seperate, logic part runs in seperate process, just like Chrome.

Outcome: Replace current Sciter sdk with Tauri for Windows/Mac/Linux

Resources:
 - Tauri project: https://github.com/tauri-apps/tauri
 - What is Sciter?: https://sciter.com/
 - Multiple windows issue: https://github.com/rustdesk/rustdesk/issues/293

Rating: Hard

Size: 350 hours

Mentor: [Carrie Chow](https://github.com/rustdesk) RustDesk author, [Heap Chen](https://github.com/Heap-Hop) RustDesk Member

### Whiteboard

Skills: Rust, Windows/Linux/Mac

Description: Whiteboard is additional collaboration tool while sharing desktop, which enables users write or draw freely on computer screen during presentations.

Outcome: Users on both side can draw on the screen of the controlled PC.

Resources:
 - Whiteboard in AnyDesk: https://anydesk.com/uk/features/whiteboard
 - Reference project: https://github.com/netless-io/flat

Rating: Hard

Size: 350 hours

Mentor: [Carrie Chow](https://github.com/rustdesk) RustDesk author

### UDP Support

Skills: Rust, TCP/IP

Description: RustDesk is using TCP hole punching for P2P connection. As we know, QUIC runs over UDP and not TCP, UDP is faster, simpler, and more efficient than TCP. RustDesk seeks to support UDP hole punching for better performance under weak network scenario.

Outcome: P2P connection over UDP.

Resources:
- Practical solution: https://github.com/Matrix-Zhang/tokio_kcp

Rating: Medium

Size: 175 hours

Mentor: [Carrie Chow](https://github.com/rustdesk) RustDesk author

### Copy/Paste file on Linux and Mac

Skills: Rust, C/C++, Objective-C, Linux/Mac

Description: RustDesk has file copy/paste support under Windows. User can copy file on one side and then paste it on the other side. Current windows implementation is based on FreeRDP.

Outcome: Users can copy/paste file between local side and remote side on Linux and Mac.

Rating: Hard

Size: 365 hours

Mentor: [Dragon Chen](https://github.com/fufesou) RustDesk member

