# FORMA

**FORMA** is 3D3D's parametric CAD platform: describe a part in words, sketch it, or build it
parametrically. You get exact OCCT geometry, ASME engineering blueprints, print checks, and
image to 3D generation, all in one desktop app.

Created by **3D3D** (Randall Marshall, New Brunswick, Canada).

## Download

Grab the latest installer from **[Releases](../../releases)**, or from
**[downloads.3d3d.ca](https://downloads.3d3d.ca/)**, which picks the right one for you.

| Platform | Package |
|---|---|
| Windows | `.exe` (setup) or `.msi` |
| macOS, Apple Silicon (M1 and later) | `.dmg` |
| Linux (Ubuntu / Debian) | `.deb` |

**Intel Macs are not covered yet.** The build is written and runs, but packaging it into a
`.dmg` currently hangs on our build machines, so there is no Intel download rather than a
broken one. It is being worked on. Apple Silicon, Windows and Linux are unaffected.

A universal binary that covers both Macs at once is not an option here: FORMA bundles a Python
runtime whose native CAD kernel wheels are published per architecture and not as universal
builds, so each architecture needs its own. That also keeps each download roughly half the size.

Install on Linux with `sudo apt install ./FORMA_<version>_amd64.deb` and FORMA appears in your
app menu. Closing the window shuts the whole app down; nothing keeps running in the background.

Builds are currently unsigned, so Windows and macOS may warn about an unknown publisher. On
Windows choose "More info" then "Run anyway"; on macOS right-click the app and choose Open.

## Provenance and credit

Much of FORMA builds on excellent open-source work. The vision and direction come from 3D3D:
pushing these together into the best possible solution for anybody in this space. Credit is
given where credit is due:

- [SketchForge-3D](https://github.com/Formsmith746/SketchForge-3D) (MIT), the interactive 3D editor FORMA's front end builds on
- [text-to-cad "CAD Skills"](https://github.com/earthtojake/text-to-cad) (MIT), the CAD core; its repo also offers public **parts libraries** worth exploring
- [build123d](https://github.com/gumyr/build123d) + [cadquery-ocp](https://github.com/CadQuery/OCP) (Apache-2.0/LGPL), the parametric B-Rep kernel
- [Microsoft TRELLIS](https://github.com/microsoft/TRELLIS) (MIT), image and text to 3D generation
- three.js, manifold3d, occt-wasm, Tauri, for rendering, booleans, in-browser geometry, and the desktop shell

## Feedback

Input and feedback are genuinely welcome. [Open an issue](../../issues) and tell us what you
think, what's missing, or what you'd build with it.
