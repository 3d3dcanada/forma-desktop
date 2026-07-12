# FORMA

**FORMA** is 3D3D's parametric CAD platform: describe a part in words, sketch it, or build it
parametrically — get exact OCCT geometry, ASME engineering blueprints, print checks, and
image→3D generation, all in one desktop app.

Created by **3D3D** (Randall Marshall, Nova Scotia, Canada).

## Download

Grab the latest installer from **[Releases](../../releases)**:

| Platform | Package | Status |
|---|---|---|
| Linux (Ubuntu/Debian) | `.deb` | ✅ available |
| Windows | `.msi` / `.exe` | coming soon |
| macOS | `.dmg` | coming soon |

Install on Linux: `sudo apt install ./FORMA_<version>_amd64.deb` — FORMA appears in your app
menu. Closing the window shuts the whole app down; nothing keeps running in the background.

## Provenance & credit

Much of FORMA builds on excellent open-source work — the vision and direction come from 3D3D:
pushing these together into the best possible solution for anybody in this space. Credit is
given where credit is due:

- [SketchForge-3D](https://github.com/Formsmith746/SketchForge-3D) (MIT) — the interactive 3D editor FORMA's front end builds on
- [text-to-cad "CAD Skills"](https://github.com/earthtojake/text-to-cad) (MIT) — the CAD core; its repo also offers public **parts libraries** worth exploring
- [build123d](https://github.com/gumyr/build123d) + [cadquery-ocp](https://github.com/CadQuery/OCP) (Apache-2.0/LGPL) — the parametric B-Rep kernel
- [Microsoft TRELLIS](https://github.com/microsoft/TRELLIS) (MIT) — image/text → 3D generation
- three.js, manifold3d, occt-wasm, Tauri — rendering, booleans, in-browser geometry, the desktop shell

## Feedback

Input and feedback are genuinely welcome — [open an issue](../../issues) and tell us what you
think, what's missing, or what you'd build with it.
