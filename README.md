# Murmurmaid

A single-file white-noise page for sleeping. Open `index.html` (or host it on GitHub Pages) on your phone and hit play.

- Keeps playing with the screen locked; phone volume buttons and lock-screen controls work.
- Presets: White, Pink, Brown, Rain, Leaves, Downpour, Ocean, Fan, Deep sea.
- Shape the sound with Color (white → pink → brown), Pitch, Drops (rain on leaves, sparse → downpour), Waves (swell depth) and Speed (swell rate).
- Save your own sounds; they live in the browser's local storage on that device.

How it works: three seamless noise loops (white, pink, brown) play through Web Audio, which loops sample-accurately, so there's no seam. Colour, pitch and waves are live gains, filters and LFOs, so every change glides instead of restarting. A silent looping `<audio>` element runs alongside: that's what the phone sees as "media playing", which gives you lock-screen controls and keeps the page from being suspended. On Safari the page also asks for the `playback` audio session, so the silent switch doesn't mute it.
