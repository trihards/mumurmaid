# mumurmaid

A single-file white-noise page for sleeping. Open `index.html` (or host it on GitHub Pages) on your phone and hit play.

- Keeps playing with the screen locked; phone volume buttons and lock-screen controls work.
- Presets: White, Pink, Brown, Rain, Ocean, Fan, Deep sea.
- Shape the sound with Color (white → pink → brown), Pitch, Waves (swell depth) and Speed (swell rate).
- Save your own sounds; they live in the browser's local storage on that device.

How it works: the noise is rendered in JavaScript into a seamless two-minute WAV loop and played through a plain `<audio>` element, rather than live Web Audio, because mobile browsers keep media elements running in the background and route them through the system volume.
