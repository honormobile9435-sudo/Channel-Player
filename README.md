# Channel Soundboard

A free, offline soundboard-style music mixer that installs like an app on **Android, iPhone and computers (Chrome / Edge)**. Works in landscape and portrait and switches layout automatically.

**Features:** waveform seek bar with elapsed/remaining time · one channel per song with its own fader, play button and output-device button · master volume · multiplay (many songs at once, one Play/Pause for all) · crossfade · previous/next · rewind/forward with fast scrub · Stop / Repeat / Continue + Shuffle · equalizer presets + bass boost · global stop timer · per-song start/stop times · total and per-song duration · move/replace/delete channels · lock-screen controls.

Songs are stored on your own device (IndexedDB) - nothing is uploaded. No ads, no accounts.

## Publish on GitHub Pages
1. Create a **Public** repository (e.g. `channel-soundboard`).
2. Upload all files from this folder (`index.html`, `sw.js`, `manifest.webmanifest`, the PNG icons, `.nojekyll`).
3. **Settings → Pages → Deploy from a branch →** `main` / `(root)` → Save.
4. After a minute: `https://<your-username>.github.io/channel-soundboard/`

## Install
- **Android (Chrome):** open the link → **Install** button in the app, or menu ⋮ → **Install app**.
- **Computer (Chrome / Edge):** open the link → **Install** button in the app, or the install icon at the right of the address bar.
- **iPhone (Safari):** Share → **Add to Home Screen**.

After the first open it works offline. Songs are saved per device/browser, so add them again on each device.

## Good to know
- **Output-device button:** works best in Chrome/Edge on a computer (speakers, Bluetooth, USB, HDMI). Phones usually expose only one output, and iPhone has none. If a device cannot be used the app says so and keeps playing on the default output.
- Timers and per-song start/stop times only run while the app is open.
- Keyboard (computer): Space = play/pause, Left/Right = 10 seconds back/forward.
- After changing files on GitHub, bump `CACHE` in `sw.js` (`soundboard-v4`, ...) so devices pick up the update.
