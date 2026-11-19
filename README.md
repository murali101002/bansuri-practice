# 🪈 Bansuri Practice

A complete bansuri (Indian bamboo flute) practice app in **one single HTML file** — `index.html`.
No frameworks, no build step, no backend, no login. Works offline once loaded. All audio stays on the device.

Built for a C bansuri beginner, with a focus on the classic Pa problem (sealing hole 6 with the right-hand ring finger).

## Use it

**Online:** open the deployed URL (Vercel), or
**Offline:** download `index.html` and open it in Chrome on your phone.

1. Open in Chrome (Android recommended) and **allow the microphone**.
2. Tap **Set Sa** → play Sa (3 holes closed) the way you normally play → tap **Set Sa from my flute**. Do this once per flute (PVC Radhe C / Wooden C profiles are saved separately).
3. Go to **Practice → Mandra → Pa** — soft air, all 6 holes closed.

## Features

- **Listen (tuner):** autocorrelation pitch detection (McLeod/MPM) tuned for breathy flute tone, median-filtered, 290–1150 Hz, cents meter with plain words, stability bar, 5-second pitch graph, and plain-language leak hints ("Pitch is jumping Pa to Dha. Check hole 6.")
- **Learn:** fingering chart for all 12 swars + Sa', half-hole diagrams for komal/teevra swars, reference tones, hole-6 coaching on Pa
- **Practice:** Target Swar (Pa only / Sa–Pa–Sa–Pa / any swar), Mandra practice (low Pa, Dha, Ni with hold goals 3/5/8/10 s), Sargam trainer with metronome (40–120 BPM)
- **Listen first:** every sequence can be demonstrated at your tempo with note highlighting before you play it
- **Rhythm game:** play along with the visual beat — 5 patterns, per-note pitch + timing score, stars, best scores saved. "Follows the beat" or "Waits for me" mode
- **Quiz:** 10 plain-language questions on swars, fingering and air; every correct answer earns XP
- **Levels & XP:** practice seconds, quiz answers and rhythm scores add up through 6 levels
- **Progress:** 7-day per-swar accuracy, best Pa hold, practice minutes, streak — all in localStorage
- **Drone:** Sa–Pa tanpura-style drone (pure fifth) with volume control
- **Tuning:** Pure (just intonation, default — matches the drone and natural bansuri scale) or Piano-style (equal temperament) — switch in Set Sa
- Large text, dark high-contrast UI, phone-on-a-stand friendly

## Note

The microphone requires a secure context — the Vercel URL (https) or opening the local file in Chrome both work. Progress and calibration live only in your browser's localStorage; nothing is uploaded anywhere.
