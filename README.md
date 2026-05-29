# Fractal Studio

A self-contained, mobile-first fractal generator that runs entirely in the browser. Open it and it renders immediately — no build step, no server, no dependencies beyond two web fonts.

**Live:** (https://tridentintelfree.github.io/TridentIntelFree/)

## Features

- **Four fractal families:** Mandelbrot, Julia, Burning Ship, Tricorn
- **Tweakable shape:** power (2–8, turns Mandelbrot/Julia into multibrots), Julia C parameters, iteration depth
- **Color controls:** 8 cosine-gradient palettes, band density, color shift, smooth-gradient toggle
- **Touch gestures:** drag to pan, pinch to zoom, double-tap to zoom in
- **Randomize** for fast art discovery
- **High-resolution PNG export** (up to ~3200 px)
- **Shareable artwork links:** the full state (type, zoom, coordinates, colors) is encoded in the URL, so any link reopens that exact composition

## Use

Open the page and start exploring. Tap **Controls** at the bottom (or use the right-hand sidebar on a wide screen) to adjust parameters. Use the **+ / − / ⟲** buttons or touch gestures to navigate.

- **Save image** renders a high-res PNG and downloads it.
- **Copy this artwork’s link** copies a URL that reopens the current fractal exactly.

## Add to Home Screen

Open the live URL in your mobile browser, then **Share → Add to Home Screen**. It launches fullscreen like a standalone app. Because each artwork lives in its own URL, you can add multiple icons that each open a different fractal.

## Privacy & offline

Everything runs locally in the browser. No data leaves the device. Once loaded, it works offline (the only external request is for the two UI fonts, which fall back to system monospace if unavailable).

## Tech

Plain HTML, CSS, and vanilla JavaScript in a single file. Fractals are computed on a `<canvas>` with direct pixel manipulation, smooth (continuous) escape-time coloring, a low-resolution preview during interaction, and a progressive full-resolution render.
