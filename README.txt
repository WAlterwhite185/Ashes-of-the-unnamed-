ASHES OF THE UNNAMED — Embeddable Web Vertical Slice
=========================================================

This /dist contains a single-file HTML prototype built to embed in Google Sites.
It implements a fast retro-3D feel (Three.js), pointer lock, audio-on-click,
basic combat (melee/parry, two spells), a handful of enemy archetypes, 3 shrines
(checkpoints), and a two-phase boss with the intended end twist (credits flow).
All assets are procedural to avoid external hosting.

What you get
------------
- index.html — all code inline (imports Three.js modules from jsDelivr CDN)
- config.json — tweakable knobs (reserved for future expansion)
- How-to-Embed.txt — copy/paste steps for Google Sites

Important notes
---------------
* The prototype pulls ES modules for Three.js from a public CDN. To fully avoid
  external CDNs, download the following files and reference them locally:
    - /libs/three.module.js
    - /libs/PointerLockControls.js
  Then replace the <script type="module"> imports with relative paths.
* Google Sites sometimes caches aggressively; force-refresh with Ctrl+F5.
* Pointer lock inside Sites usually works after user interaction. If Sites
  disables it, the game still plays (mouse look without lock is limited).

Controls
--------
WASD move • Mouse look • Shift sprint • Space jump/dodge • LMB light/heavy (hold)
RMB block/parry • E Eldritch Bolt • Q Grave Lance • R Tincture • Tab wheel (hint)
Esc pause/options • Button "Fullscreen" toggles fullscreen

Performance tips
----------------
- Keep the embed at 1280×720 for best performance.
- If the laptop is very low-powered, reduce the iframe size.
- The scene uses baked-style lambert lights, cheap fog, and no PBR.

License
-------
You may use/modify this prototype for your project. Three.js licensed under MIT.
Generated on 2025-08-31.
