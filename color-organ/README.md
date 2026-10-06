# Color Organ

A music-reactive light show that runs in the browser. It's a single HTML file with no dependencies.

Open `index.html` in Chrome, Edge, Firefox or Safari, then:

- **🖥 Use a tab (YouTube)**: reacts to the sound of another browser tab. Best option on a computer — no room noise, and it works with headphones on.
- **🎤 Use microphone**: reacts to any music playing in the room (Spotify, a speaker, a live band).
- **🎵 Load song**: plays an audio file from your device and reacts to it.

### Reacting to YouTube

Press **🖥 Use a tab (YouTube)**, choose the **Chrome Tab** tab in the picker, select your YouTube tab,
and — this is the part that is easy to miss — switch on **Also share tab audio** at the bottom left before
you click Share. Then press play on the video.

Sharing a tab this way needs Chrome or Edge; Firefox and Safari do not offer tab audio, so use the
microphone there instead. The captured sound is only analysed, never recorded or sent anywhere — the
video half of the share is discarded the moment the picker closes.

Like a classic color organ, the sound is split into three channels:
**bass (20–250 Hz) → red**, **mids (250–2000 Hz) → green**, **treble (2–12 kHz) → blue**.
Each channel's brightness follows how loud that part of the sound is. A kick drum also sets off a white flash.

## Modes
- **Blend**: three soft glows that mix across the whole screen
- **Classic**: three side-by-side light bars, like an old-school color organ
- **Spectrum**: 48 rainbow strips (log-spaced frequencies)
- **Pulse**: a center glow, plus rings that shoot out on each beat

Palettes: RGB, Sunset, Ocean, Neon, and **Night** — deep indigo, moonlit blue and a warm point of
starlight, kept dim on purpose so it works as ambient light in a dark room rather than lighting it up.
Sensitivity and smoothing sliders let you tune how it reacts.
Auto-gain adjusts to quiet and loud songs on its own.

**Keys:** `F` fullscreen · `M` next mode · `Space` play/pause. The controls hide after a few seconds without mouse movement.

## Install it as an app (phone, tablet, computer)

Color Organ is a Progressive Web App (PWA). Once it's on an `https://` address, you can install it to your home screen or desktop.
It then opens full-screen like a native app, works offline and keeps your screen on while it's running.

**It is already hosted.** GitHub Pages serves this repo from the `gh-pages` branch, and Color Organ is deployed there as a subfolder, so it is live at:

**https://tsusimiw.github.io/N8N-Automations/color-organ/**

To ship a change, copy this folder to the `gh-pages` branch under `color-organ/` and push; Pages redeploys on its own. The birthday website stays at the site root.

**Install it on each device:**
- **Android (Chrome):** open the link, then tap **⬇ Install app** in the controls (or ⋮ menu → *Install app*).
- **iPhone / iPad (Safari):** open the link, tap **Share**, then **Add to Home Screen**.
- **Windows / Mac / ChromeOS (Chrome or Edge):** open the link, then click **⬇ Install app** or the install icon in the address bar.

> Microphone access needs `https://` or `localhost`. Opening the file directly works in most browsers, or run
> `python3 -m http.server` in this folder and visit http://localhost:8000.
