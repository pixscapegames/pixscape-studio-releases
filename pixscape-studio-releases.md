# Pixscape Studio Free

## Latest public release: 0.1.0

First public MVP release of **Pixscape Studio Free**.

### Edition
**Free Edition** — free to use, including for commercial projects.

### Platforms
- Linux `.deb`

### Website
https://pixscape.games

### Bugs / feedback
bugs@pixscape.games

### Included in 0.1.0
- sprites
- animations
- particle effects
- orthogonal tiled maps
- shaders
- shader manager
- ambient / point / cone lights
- Box2D
- asset import
- preview
- automatic atlas packing
- undo / redo

---

## Upcoming in 0.1.1

### Added
- Light layers now support parallax.
- Light overlay rendering is now consistent with parallax.
- Tilesets now preserve their original layout in the asset panel.

### Changed
- Parallax values now use 2 decimal places.
- Tiled imports now preserve tileset and tile metadata instead of flattening everything as generic images.
- Tileset browsing now supports horizontal scrolling when needed to preserve the original grid layout.

### Fixed
- Fixed light layers being ignored by the parallax pipeline.
- Fixed light icon overlay not matching rendered parallax position.
- Fixed tiled imports losing original tileset structure in the asset browser.
- Fixed tileset and spritesheet import spinners resetting user-entered values on validation errors.
- Fixed tileset and spritesheet import spinner max value being limited to 256.