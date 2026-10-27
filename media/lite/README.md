# Native 2D scene captures

Recorded from the portfolio's existing World, Planet and Renderer scene, with all scene text hidden. No reference-image pixels or third-party assets were added.

- `galaxy.mp4` / `galaxy.webp`: 3840×2160, 24 fps; original galaxy/core/planets, canvas only. The final second crossfades into the start to avoid a hard dust cut.
- `graphic`, `video`, `art` MP4/WebP pairs: 1024×1024, 24 fps, 24-second rotating-world loops, mapped to the same categories as 3D.
- MP4s contain video only, H.264/yuv420p, fast-start. WebP stills remain visible if motion is reduced or video fails.
- Runtime loads and plays only visible loops. Pause, reduced motion, hidden documents, open dialogs/galleries, save-data and the user-controlled 3D preview are respected. No runtime WebGL is used for these media.
- Existing asset credits and license requirements still apply; these captures are not an independent licensing clearance.

Capture utility: `scripts/capture-lite-worlds.cjs`, run against the local Vite server. It refuses to overwrite existing MP4 outputs. First archive/remove only your own generated outputs or select a new output directory in a copied utility before a new recording. Offline encoding uses bounded decoder/encoder threads; Windows commit exhaustion can occur even with physical RAM available.
