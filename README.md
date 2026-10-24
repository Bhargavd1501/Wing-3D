# AeroLab 3D – Finite Wing Test Section

Real-time 3D wing simulator in the browser (no dependencies). A lifting-surface solver with a rolling-up vortex wake shows tip vortices, wing-tip / root stall and flow separation on a real 3D wing. Companion to AeroLab (2D) and NozzleLab.

**Live demo:** https://bhargavd1501.github.io/Wing-3D/  

- Planform: aspect ratio 2–18, taper, sweep (−20…45°), dihedral, tip twist, span; presets for rectangular, tapered, swept, elliptical, glider and low-AR wings
- Airfoils: NACA 0012 / 2412 / 4412, flat plate, custom NACA 4-digit
- Angle of attack −10…30° and speed 10–230 m/s (compressibility via Prandtl–Glauert, valid below M ≈ 0.7)
- Visualisation: rolled-up tip vortices, wake cross-section (vertical velocity), smoke filaments, pathlines, streamlines, surface Cp, section lift, separation overlay and line, surface tufts that flip in separated flow
- Live HUD: C_L, C_Di, C_D, L/D, span efficiency, lift and drag in newton, stalled span %, sim vs theory (Helmbold–Diederich lift slope, C_L²/πAR)
- Span-loading plot against the elliptical ideal, or section angle against the stall angle
- Orbit camera: drag to rotate, pinch / wheel to zoom, double-tap to reset; Iso / Top / Side / Rear / Front presets
- Auto quality mode holds about 60 FPS on phones
- Installable as a Progressive Web App (works offline after the first visit)

## Controls
Drag: orbit · pinch / wheel: zoom · ↑ / ↓ change α · ← / → rotate · Space pauses · ↺ resets the wake · ⛶ fullscreen

## Files
`index.html` (the app) · `manifest.json` · `sw.js` · `icon-192.png` · `icon-512.png`

## Install
Open the GitHub Pages link in Chrome → ⋮ menu → **Install app** (or **Add to Home screen**).

## Note
Educational and visual tool, not a full 3D Navier–Stokes solver. Lift and induced drag come from a Weissinger-type horseshoe-vortex model with a nonlinear stall curve; separation is an empirical trailing-edge model; surface Cp is approximate. Unstalled lift agrees with finite-wing theory within about 5 %.
