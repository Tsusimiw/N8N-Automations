# Color Organ

A music-reactive light show that runs in the browser. It's a single HTML file with no dependencies.

Open `index.html` in Chrome, Edge, Firefox or Safari, then:

- **🎤 Use microphone**: reacts to any music playing in the room (Spotify, a speaker, a live band).
- **🎵 Load song**: plays an audio file from your device and reacts to it.

Like a classic color organ, the sound is split into three channels:
**bass (20–250 Hz) → red**, **mids (250–2000 Hz) → green**, **treble (2–12 kHz) → blue**.
Each channel's brightness follows how loud that part of the sound is. A kick drum also sets off a white flash.

## Modes
- **Blend**: three soft glows that mix across the whole screen
- **Classic**: three side-by-side light bars, like an old-school color organ
- **Spectrum**: 48 rainbow strips (log-spaced frequencies)
- **Pulse**: a center glow, plus rings that shoot out on each beat

Palettes: RGB, Sunset, Ocean, Neon. Sensitivity and smoothing sliders let you tune how it reacts.
Auto-gain adjusts to quiet and loud songs on its own.

**Keys:** `F` fullscreen · `M` next mode · `Space` play/pause. The controls hide after a few seconds without mouse movement.

> Microphone access needs `https://` or `localhost`. Opening the file directly works in most browsers, or run
> `python3 -m http.server` in this folder and visit http://localhost:8000.
