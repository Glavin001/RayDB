# RayDB
> Raycasting Optimized Spatial Database

---

## About

### Goal

Allow for high performance raycasting to support 1080p HD rendering (1920 by 1080 = 2,073,600 pixels) at 30 Frames-Per-Second (2,073,600 pixels times 30 FPS = 62,208,000 pixels-per-second).

This is, of course, a very extreme and lofty goal. It would be nice to be able to render, in lower-res, very large scenes in real-time and move around throughout the scene.

### File Hierarchy and Terminology

- `Database` - Collection of Scenes using the same Models and Materials
  - `Scenes` - Analagous to Tables or Collections
    - `scene1` - Collection of references to Models with transformations positioning them in this Scene
    - `scene2`
    - etc...
  - `Models` - Collection of Models
    - `model1` - Combination of coordinates/points for shapes and references to their materials
    - etc...
  - `Materials` - Collection of Materials
    - `material1` - Physical characteristics of a surface
    - etc...
