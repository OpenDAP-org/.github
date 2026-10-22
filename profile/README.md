# OpenDAP

OpenDAP is a fully open-source, open-hardware digital audio player that runs 100% on Linux. It is also a general-purpose Linux gadget: accessory **HATs** mount on its back and turn it into other tools.

## Product

**OpenDAP T1** is the first device. It comes in two editions built from exactly the same design:

- **Commercial**: assembled.
- **DIY**: a kit to build yourself.

The editions differ only in manufacturing precision.

## Repositories

| Area | Repository | What it is |
|---|---|---|
| Product | [t1](https://github.com/opendap-project/t1) | Product requirements, complete assembly and system simulations of the T1 |
| Hardware | [board](https://github.com/opendap-project/board) | Main board (SBC) built around the SoC |
| | [case](https://github.com/opendap-project/case) | Rigid mechanics: core (with basic back cover), faceplate mount, HAT case |
| Faceplates | [faceplate-touch](https://github.com/opendap-project/faceplate-touch) | Default faceplate: touch display, status LED, microphone |
| | [faceplate-cassette](https://github.com/opendap-project/faceplate-cassette) | Inspired by cassette Walkmans |
| | [faceplate-classic](https://github.com/opendap-project/faceplate-classic) | Inspired by the iPod classic |
| Standard | [hat-standard](https://github.com/opendap-project/hat-standard) | HAT Case Standard for accessory developers |
| Process | [rfcs](https://github.com/opendap-project/rfcs) | Proposals for cross-repository and interface changes |
| Software | [system](https://github.com/opendap-project/system) | OpenDAP OS system software and SDK (Rust) |
| | [ui-components](https://github.com/opendap-project/ui-components) | Official UI components and design system |
| | [opendap-os](https://github.com/opendap-project/opendap-os) | The OpenDAP OS distribution: image build and releases |
| | [toolkit](https://github.com/opendap-project/toolkit) | Developer host tools (not shipped in OpenDAP OS) |
| Libraries | [kicad-lib](https://github.com/opendap-project/kicad-lib) | KiCad symbols, footprints, 3D models and fab design rules |
| | [freecad-lib](https://github.com/opendap-project/freecad-lib) | FreeCAD mechanical parts |
| | [blender-lib](https://github.com/opendap-project/blender-lib) | Blender materials, models and scenes |
| | [parts-lib](https://github.com/opendap-project/parts-lib) | Per-part spec sheets and the manifest of datasheets and vendor models |
| Official HATs | [hat-powerbank](https://github.com/opendap-project/hat-powerbank) | Powerbank |
| | [hat-nas](https://github.com/opendap-project/hat-nas) | SSD and Ethernet |
| | [hat-camera](https://github.com/opendap-project/hat-camera) | Action camera |
| | [hat-recorder](https://github.com/opendap-project/hat-recorder) | Recorder inspired by Tascam |
| | [hat-oscilloscope](https://github.com/opendap-project/hat-oscilloscope) | Oscilloscope based on the DS212 |
| | [hat-vna](https://github.com/opendap-project/hat-vna) | Vector network analyzer based on NanoVNA |
| | [hat-radio](https://github.com/opendap-project/hat-radio) | SDR based on HackRF Pro |

Faceplates are interchangeable front modules; HATs are accessories mounted on the back. Each HAT is a complete project: hardware, case, firmware, software, OpenDAP OS package, its own tooling and, where useful, on-board AI.

## Licensing

| Content | License |
|---|---|
| Hardware of OpenDAP products (schematics, PCB, mechanics) | [CERN-OHL-S-2.0](https://ohwr.org/cern_ohl_s_v2.txt) |
| Hardware building blocks others combine into their own designs: part libraries, HAT Case Standard reference designs, every `export/` folder | [CERN-OHL-W-2.0](https://ohwr.org/cern_ohl_w_v2.txt) |
| Software | [GPL-3.0-or-later](https://www.gnu.org/licenses/gpl-3.0.html) |
| Software libraries others build on: SDK, design system, schemas | [MPL-2.0](https://www.mozilla.org/MPL/2.0/) |
| Firmware, project templates | [MIT](https://opensource.org/license/mit) |
| Documentation, specifications, manuals, renders, project assets | [CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Generic shared assets others can build on (`blender-lib/shared/`) | [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/) |

Changes to anything OpenDAP publishes stay open. What others build on top (their own hardware, firmware or software) is theirs to license.

Every repository follows the [REUSE](https://reuse.software) layout, so each file's license is machine-readable.

## Conventions

- Everything in the repositories is written in English.
- Each repository keeps its confirmed context in `docs/`: requirements first, then Architecture Decision Records (ADRs) for decisions already taken.
