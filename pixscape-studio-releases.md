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

## Included in 0.1.1 (latest)

### Added
- Added parallax support for light layers.
- Added light parallax handling in overlay rendering.
- Added dedicated TILE and TILESET asset metadata support for tiled imports.
- Added fixed tileset layout mode in the asset thumbnails view to preserve original tileset arrangement.
- Added transform property historization in `TransformPanel`.
- Added `EditTransformCommand` with undo/redo support for position, rotation, scale, and origin edits.
- Added `ORIGIN` support to `TransformOp`.
- Added preview save guard for persistent non-historized scene/layer changes before launching preview.

### Changed
- Requires pixscape-runtime 0.1.1 or later for light layer parallax support.
- Light layers now use `LayerParallaxComponent` like classic and tiled layers.
- Updated editor overlay behavior to stay consistent with parallax.
- Parallax now uses 2 decimal places.
- Tiled asset imports now persist tilesets and tiles with dedicated metadata instead of flattening everything as generic images.
- The asset panel now preserves original tileset ordering when browsing a tileset subfolder.
- Tileset browsing now supports horizontal scrolling when needed to preserve the original grid layout.
- Transform property fields now always resync from the model after commit instead of trusting raw typed text.
- Programmatic text updates in numeric/text property widgets now bypass destructive input filtering.

### Fixed
- Fixed light layers being ignored by the parallax pipeline.
- Fixed light icon overlay not matching rendered parallax position.
- Fixed tiled imports losing original tileset structure in the asset browser.
- Fixed spritesheet and tileset import spinners resetting user values on validation errors.
- Fixed spritesheet and tileset import spinner maximum being too low (256).
- Fixed negative `scaleX` / `scaleY` not flipping sprites correctly at render time.
- Fixed transform X/Y values becoming positive after field validation or commit.
- Fixed negative values being lost in `FloatField` and `IntField` during refresh/commit/programmatic updates.
- Fixed transform properties not being undoable from the properties panel.
- Fixed origin edits not being propagated through transform property refresh dispatch.
- Fixed preview potentially using stale exported data when scene/layer persistent changes were not tracked by history.