<p align="center">
  <img src="pixscape_logo.png" alt="Pixscape logo" width="80">
</p>

<h1 align="center">Pixscape Studio Releases</h1>
<p align="center"><strong>Public release repository for Pixscape Studio binaries.</strong></p>
<br>

Pixscape Studio is a lightweight 2D game editor focused on fast iteration, tiled workflows, shaders, lights, animation, particles, and Box2D-based gameplay authoring.

## Status

Current public release: **0.1.2**

Pixscape Studio is currently available **free of charge**.

Pixscape Studio is still evolving and should currently be considered an early public release.

This repository is a **distribution repository** for Pixscape Studio binaries.  
It does **not** contain the Pixscape Studio source code.

## Downloads

Releases are published in the **Releases** section of this repository.

Current distribution targets for **0.1.2**:
- Linux: `.deb`
- Windows: `.zip`

## Included in 0.1.2

Pixscape Studio 0.1.2 expands the editor with stronger tiled workflows, broader Box2D authoring, better import ergonomics, and improved day-to-day usability.

### Main highlights
- improved import management with new layout, filtering, directory import, and better error handling
- copy / cut / paste
- alignment toolbar
- isometric tiled map support
- tiled tile transformations:
  - flip horizontal
  - flip vertical
  - rotate left
  - rotate right
- transformed tile ghost preview in Tiled mode
- tiled animations support
- extended Box2D joint editing:
  - Distance
  - Revolute
  - Prismatic
  - Wheel
  - Friction
  - Motor
  - Weld
  - Pulley
  - Gear
- better layer tooling, including applying visibility and lock checkboxes to all layers
- canvas selection now stays aligned with the Item Tree by activating the corresponding layer automatically

### Improvements
- faster Tiled Fill on large maps
- smoother Tiled brush painting during fast mouse movement
- smoother preview panning on tiled maps
- tile transformations preserved across brush, rect, and fill tools
- undo / redo in Tiled mode fully restores transformed tiles
- tiled preview reflects the exact final tile transform before painting

### Fixes
- entity names could become non-editable
- scenes could be saved when changing scenes even if they were not dirty
- images smaller than the 2048×2048 limit could be rejected during import
- `.json.bak` files were not deleted when deleting a scene
- Tiled Fill could ignore tile transformations when replacing tiles

## Runtime

Pixscape Studio is built around **Pixscape Runtime**, which is published separately as an open-source runtime library.

- Runtime repository: https://github.com/pixscapegames/pixscape-runtime
- Website and documentation: https://pixscape.games

Pixscape Studio and Pixscape Runtime do not have the same role:

- **Pixscape Studio** is the editor application and is distributed here as proprietary software
- **Pixscape Runtime** is the game-side runtime library and is published separately under its own open-source license

## Documentation

Project website:
- https://pixscape.games

Documentation and guides are published on the website.

## License

Pixscape Studio is **proprietary software**.

This repository publishes binaries only.  
The source code is not provided here and is not licensed under an open-source license.

Use of the binaries is governed by the terms in [`LICENSE.txt`](./LICENSE.txt).

## Third-party notices

Third-party license notices are listed in [`THIRD_PARTY_NOTICES.txt`](./THIRD_PARTY_NOTICES.txt).

## Support / bugs

For bug reports:
- bugs@pixscape.games

Please include:
- Pixscape Studio version
- operating system
- reproduction steps
- screenshots or logs when relevant