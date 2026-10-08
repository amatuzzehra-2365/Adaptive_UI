# AdaptiveUI: an interface that notices how you use it

A single-file, multimodal web interface that adapts its color, shape, spacing and behavior to the way you interact with it: mouse, hover, click, typing, touch, keyboard or voice.

**Live demo:** `https://amatuzzehra-2365.github.io/adaptive-ui/`

## What it does

The page watches your input and responds in real time. A central orb changes shape for each input type, and the rest of the interface adjusts around it.

| Input | What adapts |
|---|---|
| Mouse | The orb follows your pointer slightly |
| Hover | The orb morphs and the accent color shifts |
| Click | A ripple appears and the accent color changes |
| Typing | The orb stretches as you type, and the interface focuses on text |
| Touch | Buttons, text area and cards get larger and rounder |
| Keyboard | Focus rings become thick and clearly visible |
| Voice | The orb pulses while listening and speech is turned into commands |

## Commands (typed or spoken)

- **Colors:** `red`, `blue`, `green`, `purple`, `orange`, `pink`, `yellow`, `teal`
- **Theme:** `dark`, `light`
- **Size:** `bigger`, `smaller`
- **Reset:** `reset` (or press `Esc`)

A color you choose stays pinned until you reset, so it isn't overwritten by the next hover or click.

## Features

- Live "Detected inputs" panel with a counter per input type
- Timestamped activity log
- Dark/light toggle that respects your system preference
- Live interim text while speaking, and a clear message if the mic is blocked
- Keyboard accessible, with visible focus and `prefers-reduced-motion` support
- Responsive down to mobile
- Fixes for touch/mouse event conflicts and whole-word command matching

## Run it

No build step and no dependencies.

1. Download `index.html`.
2. Open it in a browser.

For voice input, use **Chrome or Edge** and serve the page over HTTPS (GitHub Pages does this) or from `localhost`. Firefox does not support the Web Speech API.

## Deploy on GitHub Pages

1. Put the file in the repo root as `index.html`.
2. Go to **Settings → Pages**.
3. Set Source to **Deploy from a branch**, then choose `main` and `/ (root)`.
4. Save, and your site will be live in a minute or two.

## Tech

- HTML, CSS and vanilla JavaScript in one file
- CSS custom properties with `color-mix()` for theming
- Web Speech API for voice recognition
- Google Fonts: Bricolage Grotesque and Instrument Sans

## Browser support

| Feature | Chrome / Edge | Safari | Firefox |
|---|---|---|---|
| Interface and adaptation | Yes | Yes | Yes |
| Voice commands | Yes | Partial | No |

## Ideas for next steps

- Urdu and multi-language voice commands
- Sound feedback for each input type
- Saving the chosen theme between visits
- Audio-reactive orb using microphone volume

## License

MIT. Use it, change it, share it.
