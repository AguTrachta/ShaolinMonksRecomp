# Shaolin Monks Recomp

<p align="center">
  <img src="docs/images/shaolin-monks-recomp.png" width="760" alt="Shaolin Monks Recomp logo">
</p>

<p align="center">
  <a href="https://github.com/OAleex/ShaolinMonksRecomp/releases"><img src="https://img.shields.io/badge/Download-Windows_x64-2563eb?style=for-the-badge&amp;logo=windows11&amp;logoColor=white" alt="Download for Windows x64"></a>
  <a href="https://github.com/OAleex/ShaolinMonksRecomp/releases"><img src="https://img.shields.io/github/downloads/OAleex/ShaolinMonksRecomp/total?style=for-the-badge&amp;logo=github&amp;label=Release%20downloads" alt="Total GitHub release downloads"></a>
  <a href="https://github.com/OAleex/ShaolinMonksRecomp/releases"><img src="https://img.shields.io/github/v/release/OAleex/ShaolinMonksRecomp?include_prereleases&amp;sort=semver&amp;style=for-the-badge&amp;label=Latest%20release" alt="Latest GitHub release, including prereleases"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-GPL--2.0--or--later-blue?style=for-the-badge" alt="GPL-2.0-or-later license"></a>
</p>

> [!IMPORTANT]
> Shaolin Monks Recomp does not include the original game or its assets.
> You must provide your own legally obtained **USA/Europe Xbox copy of Mortal Kombat: Shaolin Monks**.

**A native Windows PC port of Mortal Kombat: Shaolin Monks, made through static recompilation.**

The original Xbox code runs directly on the PC, without an Xbox emulator, with graphics through Direct3D 12.
The port adds resolution and render scale settings, display modes, keyboard and mouse input, and remappable controller buttons.

The campaign is playable from start to finish. Some graphical issues remain, with fixes planned for future builds.

**Bonus content:** **Mortal Kombat II** and **The Suffering Demo** are not playable yet. Support is planned for a future update.

## System requirements

| Component | Requirement |
| --- | --- |
| CPU | x64 processor with SSE4.2 and POPCNT |
| GPU | Direct3D 12-compatible GPU |
| Input | Keyboard and mouse, or a compatible controller |
| Game files | Original USA/Europe Xbox release |

## Platform support

| Operating system | Status |
| --- | --- |
| Windows 10 x64, version 1903 or later | Supported |
| Windows 11 x64 | Supported |
| Linux x86_64 | Coming soon |
| macOS | Not supported yet |

## Getting started

1. Extract the Windows release ZIP.
2. Run `ShaolinMonksRecomp.exe`.
3. Select your ISO, XISO, ZIP, extracted game folder, or `default.xbe`.
4. Choose your settings, then select **Save and Play**.

ISO and XISO images are read directly. ZIP contents are imported once.
Keep the selected image or complete game folder available. You can change it in the launcher's **Files and support** tab.

## Controls

Xbox, PlayStation, and other SDL-compatible controllers support connection and disconnection during play.
DualShock 4 works through USB or Bluetooth. The game displays Xbox button prompts.

| Xbox input | Keyboard | Mouse | PlayStation |
| --- | --- | --- | --- |
| Left stick | W / A / S / D | - | Left stick |
| Direction pad | Arrow keys | - | Direction pad |
| A | Space | - | Cross |
| B | Esc or Ctrl | Right button | Circle |
| X | J | Left button | Square |
| Y | K | Middle button | Triangle |
| White | Q | Side button 2 | L1 |
| Black | C | Side button 1 | R1 |
| Left trigger | Shift | - | L2 |
| Right trigger | E | - | R2 |
| Start | Enter | - | Options |
| Back | Backspace | - | Share |
| Right stick | - | Movement | Right stick |
| FPS and frame time | F9 | - | - |
| Release / capture pointer | F10 | Click to capture | - |

See [controller settings](docs/CONTROLLERS.md) for mappings, vibration, and connection details.

## Languages

| Language | Interface | Subtitles | Voice acting |
| --- | --- | --- | --- |
| English | Yes | Yes | Yes |
| French | Yes | Yes | Yes |
| German | Yes | Yes | Yes |
| Spanish | Yes | Yes | Yes |
| Italian | Yes | Yes | Yes |
| Brazilian Portuguese | Coming soon | Coming soon | Coming soon |

## User files

| Data | Default location |
| --- | --- |
| Saves | Windows Saved Games folder: `Shaolin Monks\hdd` |
| Configuration | `%LOCALAPPDATA%\Shaolin Monks Recomp\settings.toml` |
| Logs | `%LOCALAPPDATA%\Shaolin Monks Recomp\logs` |
| Crash reports | `%LOCALAPPDATA%\Shaolin Monks Recomp\crashes` |

Error messages identify the session log. Closing the message opens `%LOCALAPPDATA%\Shaolin Monks Recomp`.
Include that log when you report a problem.

## Credits

- [TGP482 / XboxXBERecomp](https://github.com/TGP482/XboxXBERecomp): static recompiler and Xbox runtime.
- [LLVM / Clang](https://llvm.org/): native code compilation.
- [Ghidra](https://github.com/NationalSecurityAgency/ghidra): executable analysis and function inspection.
- [SDL](https://github.com/libsdl-org/SDL): controller input and device detection.
- [Dear ImGui](https://github.com/ocornut/imgui): host interface and performance display.
- [toml++](https://github.com/marzer/tomlplusplus): configuration files.
- [miniz](https://github.com/richgel999/miniz): ZIP imports.
- [xemu](https://xemu.app/), [Cxbx-Reloaded](https://github.com/Cxbx-Reloaded/Cxbx-Reloaded), and [nxdk](https://github.com/XboxDev/nxdk): behavior and ABI references.

See [BUILDING.md](docs/BUILDING.md) to build from source, or [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) to report a problem.

## AI usage

The development process uses AI assistance for executable analysis, code changes, debugging, tests, build scripts, and documentation.
The maintainer reviews these contributions. Validation includes automated tests and gameplay checks.

## License

The project code uses **GPL-2.0-or-later**. See [LICENSE](LICENSE), [tools and dependencies](UPSTREAM.md), and [dependency notices](licenses).
The project license does not grant rights to the original game or its artwork.
This project is not affiliated with or endorsed by the owners of Mortal Kombat or Xbox.
