# Alien Intercept

A static HTML canvas shooter prototype.

- Canvas renders the game scene.
- htmx swaps mission panel fragments.
- Pretext is used for canvas radio text when available.
- Chromium's experimental `drawElementImage()` path is used when enabled; otherwise the HUD uses a DOM overlay fallback.

Run locally with any static file server.

## Enable HTML-in-Canvas

The game works without this flag by using a DOM overlay fallback. To try the experimental native HTML-in-Canvas path in Chrome or Chromium:

1. Open `chrome://flags/#canvas-draw-element`.
2. Set `Canvas 2D drawElement` to `Enabled`.
3. Restart the browser.
4. Open the game again.

If the flag is not available, use Chrome Canary or a newer Chromium build.
