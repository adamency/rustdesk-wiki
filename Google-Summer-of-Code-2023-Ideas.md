RustDesk project would like to participate in Google Summer of Code 2023.

https://github.com/rustdesk/rustdesk/wiki/Google-Summer-of-Code-2023

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
RustDesk chose Sciter (stable version) and Flutter (nightly build) as its Desktop UI SDK. As Tauri turns to be stable, it is time to switch to a more elegant UI SDK. Current RustDesk UI is based on TIScript+html+css, TIScript is a modified version of Javascript, and we also have an unfinished sciter-js branch.

Outcome: Replace current Sciter sdk with Tauri for Windows/Mac/Linux

Resources:
 - Tauri project: https://github.com/tauri-apps/tauri
 - What is Sciter?: https://sciter.com/
 - Sciter-js branch: https://github.com/rustdesk/rustdesk/tree/sciterjs

Rating: Hard

Size: 350 hours

Mentor: [Kingtous](https://github.com/kingtous) RustDesk Member, [Heap Chen](https://github.com/Heap-Hop) RustDesk Member

### Whiteboard

Skills: Rust, Windows/Linux/Mac

Description: Whiteboard is additional collaboration tool while sharing desktop, which enables users write or draw freely on computer screen during presentations.

Outcome: Users on both side can draw on the screen of the controlled PC.

Resources:
 - Whiteboard in AnyDesk: https://anydesk.com/uk/features/whiteboard
 - Issue: https://github.com/rustdesk/rustdesk/issues/425

Rating: Hard

Size: 350 hours

Mentor: [Carrie Chow](https://github.com/rustdesk) RustDesk author

### WebRTC Support

Skills: Rust, WebRTC

Description: RustDesk is using TCP hole punching for P2P connection. WebRTC is a more common protocol, WebRTC support make RustDesk more universal, and it can also improve the performance of RustDesk web client.

Outcome: RustDesk over WebRTC

Resources:
- https://github.com/webrtc-rs/webrtc

Rating: Hard

Size: 350 hours

Mentor: [Carrie Chow](https://github.com/rustdesk) RustDesk author

### Copy/Paste file on Linux and Mac

Skills: Rust, C/C++, Objective-C, Linux/Mac

Description: RustDesk has file copy/paste support under Windows. User can copy file on one side and then paste it on the other side. Current windows implementation is based on FreeRDP.

Outcome: Users can copy/paste file between local side and remote side on Linux and Mac.

Rating: Hard

Size: 350 hours

Mentor: [Dragon Chen](https://github.com/fufesou) RustDesk member
