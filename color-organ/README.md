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

## Install it as an app (phone, tablet, computer)

Color Organ is a Progressive Web App (PWA). Once it's on an `https://` address, you can install it to your home screen or desktop.
It then opens full-screen like a native app, works offline and keeps your screen on while it's running.

**1. Host it (one time, free).** In this GitHub repo, go to **Settings → Pages**. Under *Build and deployment*, set Source to **Deploy from a branch**, then pick the branch (`main` once this is merged) and `/ (root)`. Click Save.
After a minute or so it's live at:
`https://tsusimiw.github.io/N8N-Automations/color-organ/`

**2. Install it on each device:**
- **Android (Chrome):** open the link, then tap **⬇ Install app** in the controls (or ⋮ menu → *Install app*).
- **iPhone / iPad (Safari):** open the link, tap **Share**, then **Add to Home Screen**.
- **Windows / Mac / ChromeOS (Chrome or Edge):** open the link, then click **⬇ Install app** or the install icon in the address bar.

> Microphone access needs `https://` or `localhost`. Opening the file directly works in most browsers, or run
> `python3 -m http.server` in this folder and visit http://localhost:8000.
