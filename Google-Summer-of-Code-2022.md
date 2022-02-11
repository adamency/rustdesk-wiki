List of project ideas for contributors applying to the Google Summer of Code program in 2022 (GSoC 2022).

## Timeline

Until March 7 - 18:00 UTC, 2022 we won't know if we will have been accepted to be part of GSoC.

Please always refer to the [official timeline](https://developers.google.com/open-source/gsoc/timeline). 
  
## Application Process

#### 0. Get familiar with GSoC

First of all, and if you have not done that yet, read [How it Works](https://summerofcode.withgoogle.com/how-it-works) which will allow you to understand all this process and how the program works overall.
  
#### 1. Discuss the project idea with the mentor(s)

This is a required step unless you have dived in into the existing codebase and understood everything perfectly (very hard) and the idea you prefer is on the list below.

If your idea is not listed, please discuss it with the mentors in the available [contact channels](https://github.com/rustdesk/rustdesk/wiki/Google-Summer-of-Code-2022#find-us). We're always open to new ideas and won't hesitate on choosing them if you demonstrate to be a good candidate!  
  
#### 2. Understand that

- You're committing to a project and we may ask you to publicly publish your weekly progress on it.
- It's the first year Metacall is joining the GSoC program and we will ask you to give feedback on our mentorship and management continuously.
- You wholeheartedly agree with the [code of conduct](https://github.com/rustdesk/rustdesk/blob/master/CONTRIBUTING.md).
- You must tell us if there's any proposed idea that you don't think would fit the timeline or could be boring (yes, we're asking for feedback).
  
#### 3. Fill out the application form

We recommend you to follow [Google's guide to Writing a Proposal](https://google.github.io/gsocguides/student/writing-a-proposal) as we won't be too harsh on the format and we won't give any template. But hey, we're giving you a starting point!

You can send the proposal link to any readable format you wish: Google Docs, plain text, in markdown... and preferably hosted online, accessible with a common browser **without downloading anything locally**.

You can also ask for a review anytime to the community or mentor candidates before the student application deadline. It's much easier if you get feedback early than to wait for the last moment.
  

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

