# 🎵 Sound Sculpture Player

An interactive 3D audio visualizer with a full-featured music player. Drop any track and watch a living 3D sculpture respond to every beat, bass hit, and frequency shift — in real time, right in your browser.

## 🖼️ Preview

![Sound Sculpture Player — upload screen](thumbnail.png)

![Sound Sculpture Player — active](thumbnail2.png)

![Sound Sculpture Player — playlist](thumbnail3.png)

## ✨ Features

- **Playlist** — load multiple tracks at once, manage your queue on the fly
- **Full player controls** — play, pause, stop, previous, next
- **Loop & Shuffle** — repeat a single track or go full random
- **Seekbar** — click anywhere on the progress bar to jump to that moment
- **Volume control** — smooth slider with instant response
- **3D sculpture** — a sphere that deforms in real time based on audio frequencies
- **Orbital rings** — two rings that pulse and scale with the music
- **Particle field** — a cloud of particles that reacts to bass
- **Dynamic lighting** — four colored lights that shift intensity with the beat
- **Drag & drop** — just drop your files onto the page

## 🚀 How to use

1. Open `index.html` in your browser
2. Drag & drop audio files or click to select them (MP3, WAV, OGG, FLAC, M4A)
3. The 3D sculpture starts reacting to the music immediately
4. Add more tracks anytime via the playlist panel
5. Use the player controls at the bottom to navigate your queue

## 🔬 How it works

The app uses the **Web Audio API** to run a real-time FFT analysis on the audio stream. The frequency data is split into three bands:

- **Bass (0–8%)** — drives the sphere deformation and particle expansion
- **Mids (8–35%)** — controls ring rotation speed and wireframe opacity  
- **Highs (35–100%)** — affects particle opacity, size, and light intensity

All of this is rendered via **Three.js** using WebGL — no canvas 2D, no SVG.

## 🛠️ Built with

- [Three.js r128](https://threejs.org/) — 3D rendering via WebGL
- [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) — real-time frequency analysis
- Vanilla JavaScript — player engine, playlist logic, UI
- HTML5 / CSS3 — layout and styling

> 100% client-side. No backend, no dependencies to install. Works fully offline.

## 📁 Files

```
sound-sculpture-player/
├── index.html       ← entire app, self-contained
├── thumbnail.png    ← upload screen
├── thumbnail2.png   ← active player
└── README.md
```