## Project Ideas

### Wayland Support

Skills: Rust, C/C++, Linux

Description:
RustDesk support X11 on Linux, but does not support Wayland yet. Wayland has totally different API for screen capture and keyboard/mouse input compared with X11. Wayland has strict permission control, you can only capture screen under the user session. A permission dialog will pop up once you initiates screen capture, this causes big problem for remote control scenario.

Resources:
 - Discuss on Wayland support: https://github.com/rustdesk/rustdesk/issues/56
 - Initial job done for Wayland, only screen capture: https://github.com/rustdesk/rustdesk/tree/master/libs/scrap/src/wayland

## Find Us

<a href="https://t.me/rustdesk1116" alt="Telegram">Telegram</a>

<a href="https://discord.com/invite/nDceKgxnkV" alt="Discord">Discord</a>
