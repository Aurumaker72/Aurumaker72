## About Me

I'm a software developer with a knack for elegant, performant, and user-respecting software.

Most of my OSS contributions focus on interaction and systems design.

## Activity

Here's where I usually toil at least semi-actively:

[Mupen64](https://github.com/mupen64/mupen64-rr-lua) as lead maintainer since 2021

[SM64LuaRedux](https://github.com/mupen64/SM64LuaRedux) as lead maintainer since 2023

[ugui](https://github.com/mupen64/ugui) as lead maintainer since 2023

[Key2Joy](https://github.com/Key2Joy/Key2Joy) as a somewhat active co-maintainer since 2025

[TAS Comp Bot](https://github.com/bxrru/TAS-Comp-Bot) as a contributor

[Constructorium Games](https://github.com/Constructorium-Games) as a founder

## History

Want to learn some history about obscure software? Sure you do!

### Mupen64

Mupen64 is a TASing[^1] emulator for the Nintendo 64.

My work here began with minor QoL improvements and grew into iteratively re-architecting the entire project to a workable codebase.

With the architectural groundwork laid, my focus shifted to feedback-driven major feature development, QoL, and performance.

Mupen64 requires plugins for its emulation core to function. For a long time, the only option was a partially closed-source plugin set that decayed with each Windows update.

In September 2025, work began to remedy this by finding 4 open-source plugins (for a full plugin set, thanks to [Crackhex](https://github.com/Crackhex) for finding the RSP plugin) and gradually adapting them to modern requirements.

By January 2026, the plugin modernization project was finalized. We now have a reliable and highly performant plugin set with much lower maintenance overhead.

Due to its tooling ecosystem and relative ease of use, Mupen64 remains the preferred emulator for Super Mario 64 TASing.

### SM64LuaRedux

SM64LuaRedux is a Lua workspace for Super Mario 64 TASing that runs inside Mupen64.

I started this project as an experiment based on [mkdasher's SM64Lua](https://github.com/mkdasher/SM64Lua) that leveraged [ugui](https://github.com/mupen64/ugui) for GUI with only minor improvements and visual changes.

Upon noticing the dispersed Super Mario 64 TAS Lua tooling ecosystem, I pivoted this project to something resembling an "everything script".

The tools were merged and made accessible while also leveraging new Mupen64 APIs to improve performance, with the added benefit of consistent upstream UI/UX improvements from ugui. 

In 2025, [FramePerfection](https://github.com/FramePerfection) implemented "Semantic Workflow", a revolutionary TASing workflow that allows higher-level strategy development and greatly speeds up the TASing process. 

### ugui

ugui is an immediate-mode GUI framework for Lua. It also implements a renderer abstraction called `BreitbandGraphics`, which provides a backend for rendering in Mupen64 using Direct2D.

This project was born because I couldn't find any immediate-mode Lua GUI library that was trivial to include in a project, hackable, and had an easy-to-understand API.

ugui is currently undergoing major changes to introduce a WPF-like layout system. I'll update this section with new developments!

[^1]: https://en.wikipedia.org/wiki/Tool-assisted_speedrun
