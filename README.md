# Ned's portfolio: haoqi.design-inspired motion prototype

A prototype of the work gallery + hero, separate from the live portfolio. Inspired by [haoqi.design](https://haoqi.design/).

| Idea | Borrowed from haoqi.design | Here |
|---|---|---|
| Inertial smooth scroll | Lenis | Lenis 1.1.13, anchors offset for the sticky header |
| WebGL image planes synced to DOM placeholders | one fixed canvas, a textured quad per card | three.js r128, scroll-velocity bend, hover ripple + RGB shift, reveal-in, rounded-corner shader |
| Layout + type | alternating full/half cards, mono caption row, crosshair marks, giant uppercase heading | same, in Ned's pastel clay palette |
| Cursor | glossy 3D pointer | gloss blob that lerps and says OPEN over cards |

Cards stay real links; with WebGL off or `prefers-reduced-motion` the normal `<img>` shows.

Run: `python3 -m http.server` then open http://localhost:8000
