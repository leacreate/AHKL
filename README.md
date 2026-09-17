# AHKL — AutoHotkey for Linux

> 🐧 A Linux-focused, AutoHotkey-style automation runtime with GUI tools, script translation, global hotkeys, gaming support, and `/dev/uinput` input injection.

## 🤖 Vibe-coded / AI-assisted

**This project is explicitly vibe coded.**

AHKL was created with substantial assistance from AI during development. Code was generated, modified, debugged, and structured with AI assistance. It is an experimental project and may contain bugs, rough edges, or code that could be improved.

This repository is published as-is for experimentation, learning, and development. **Do not assume the code has been professionally audited.**

## What is AHKL?

AHKL aims to bring an AutoHotkey-like scripting experience to Linux. It includes a Python runtime/interpreter, a graphical control center, an AHK-to-AHKL translator, desktop integration, process management, and Linux input support through `evdev` and `/dev/uinput`.

The project is particularly aimed at Linux desktop automation and gaming environments, including native applications and Flatpak applications.

## Features

- AutoHotkey-style hotkeys and commands
- `.ahk` / `.ahkl` script execution
- Global keyboard and mouse event handling
- `/dev/uinput` virtual input support
- `evdev` device/event monitoring
- GUI control center
- Macro process manager
- Emergency kill switch
- Windows AHK → Linux AHKL translator
- Desktop/file-association installer
- Example scripts
- Test suite

## Arch Linux

AHKL is developed with Arch Linux in mind and should also be suitable for Arch-based distributions such as CachyOS, depending on the installed dependencies and system configuration.

### Dependencies

At minimum, the Python package dependencies include:

```bash
python
python-pip
python-evdev
```

## Quick start

From the project directory:

```bash
python -m pip install -e .
```

Then:

```bash
ahkl gui
```

or run a script directly:

```bash
ahkl run examples/roblox_sober_macro.ahk
```

## Useful commands

```bash
ahkl gui
ahkl run <script.ahk>
ahkl kill-all
ahkl ps
ahkl install-desktop
ahkl translate <script.ahk> -o <script.ahkl>
ahkl doctor
ahkl list-devices
ahkl test-keys
```

## Safety / permissions

Input injection and global event monitoring can require access to Linux input devices. Only run scripts you understand and trust. AHKL can generate keyboard/mouse input, so a badly written script can cause unexpected actions.

## Project status

AHKL is an experimental, vibe-coded project. APIs and behavior may change, and some features may still be incomplete.

## Source archive

The original uploaded project is preserved in the repository as `AHKL-source.zip`.

## License

No license has been declared yet. Until a license is added, normal copyright restrictions apply to the repository contents.
