# Google Summer of Code 2022
List of project ideas for contributors applying to the Google Summer of Code program in 2022 (GSoC 2022).

## Timeline

Until March 7 - 18:00 UTC, 2022 we won't know if we will have been accepted to be part of GSoC.

Please always refer to the [official timeline](https://developers.google.com/open-source/gsoc/timeline). 
  
## Application Process

#### 0. Get familiar with GSoC

First of all, and if you have not done that yet, read [How it Works](https://summerofcode.withgoogle.com/how-it-works) which will allow you to understand all this process and how the program works overall.
  
#### 1. Discuss the project idea with the mentor(s)

This is a required step unless you have dived in into the existing codebase and understood everything perfectly (very hard) and the idea you prefer is on the list below.

If your idea is not listed, please discuss it with the mentors in the available [contact channels](https://github.com/metacall/gsoc-2021#find-us). We're always open to new ideas and won't hesitate on choosing them if you demonstrate to be a good candidate!  
  
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

### Embedding LLVM (LLVM Loader)

Skills: C++

Description:
The LLVM Project is a collection of modular and reusable compiler and toolchain technologies. Implementing LLVM into MetaCall will allow languages which have LLVM backend or can compile to LLVM IR. This will provide support to other loaders in the future like C/C++ Loader that can be implemented with `clang`, a frontend for LLVM.

Resources:
 - LLVM Embedding Manual: https://llvm.org/docs/CMake.html#embedding-llvm-in-your-project
 - LLVM Interpreter Example for Dynamic Compilation: https://github.com/llvm/llvm-project/blob/main/llvm/tools/lli/lli.cpp
 - How to list functions in LLVM (for introspection): https://github.com/mull-project/mull/blob/35f83655b04341b6260c5358168c4ac2da7bd86d/lib/Rust/RustTestFinder.cpp#L108

### Embedding Julia language (Julia Loader)

Skills: C, C++ (optional) and Julia (at least its type system)

Description:  
Julia is a modern programming language which features performance nearly as fast as C while still being adequate to the scientific community's rapid prototyping needs. Julia has a C api that Metacall could use to connect it with other languages than C/C++ with less effort.

Resources: 
 - Julia Embedding Manual: https://docs.julialang.org/en/v1/manual/embedding/
 - Julia Dependency in CMake: https://github.com/JuliaInterop/libcxxwrap-julia/blob/master/FindJulia.cmake

### Embedding Kind Proof Assistant (Kind Loader)

Skills: Formal Verification / Proof Assistants, JavaScript (and C/C++ is a plus)

Description:  
Kind is a modern programming language that allows the developer to write formal proofs to validate the code. MetaCall has already very good support for JavaScript and formality could be implemented on top of it due to it having a [JavaScript compiler](https://github.com/moonad/FormCoreJS/blob/master/FmcToJs.js). The already implemented TypeScript Loader can be an example to follow due to TypeScript being also compiled to JavaScript. Applications would benefit from calling Kind with MetaCall, getting easy access to formal verification without having to reimplement much of the business logic and being able to verify single functions easily.

Resources:
 - Kind GitHub Repository: https://github.com/uwu-tech/Kind
 - Kind JavaScript Backend: https://github.com/uwu-tech/Kind/tree/master/bin/js
 - MetaCall TypeScript Loader (can be used as example to implement the Kind Loader): https://github.com/metacall/core/tree/develop/source/loaders/ts_loader
 - MetaCall Kind Loader Base: https://github.com/metacall/core/blob/cd843ef37fe2efcfb33bbb64dccf0973b52e8493/source/loaders/kind_loader/parsing_kind_terms.js

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

