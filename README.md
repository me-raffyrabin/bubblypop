# 🫧 BubblyPop

> Pop watery floating bubbles, uncover hidden golden-ratio spheres, and beat the clock.

![game](https://img.shields.io/badge/game-bubble--pop-6cd4ff)
![javascript](https://img.shields.io/badge/vanilla-JS-f7df1e)
![three.js](https://img.shields.io/badge/three.js-r160-000000)
![web audio api](https://img.shields.io/badge/Web%20Audio%20API-soft%20pops-ff7eb6)
![no build](https://img.shields.io/badge/build-zero%20steps-22c55e)
![license](https://img.shields.io/badge/license-MIT-blue)

**BubblyPop** is a playful, mobile-friendly browser game built with **zero build steps** — just open the HTML and play. Twenty-five fluid, watery bubbles drift up your screen. Five of them secretly hide a glowing, color-coded 3D **golden-lattice sphere**. Find all five before the 60-second timer runs out and you win!

Everything runs in a single self-contained file: synthesized pop sounds (Web Audio API), watery SVG textures, and animated 3D spheres (Three.js) — no assets to download.

---

## 🌐 Live Demo

▶️ **[Play BubblyPop now!](https://me-raffyrabin.github.io/bubblypop/)**

> Hosted on GitHub Pages — works right in your browser, no install needed. Best on a device with sound on. 🔊
>
> _Not live yet?_ Push the repo to GitHub, then go to **Settings → Pages**, set the source to your `main` branch (root), and your demo will appear at the link above.

---

## ✨ Features

- 🫧 **25 fluid bubbles** with a smooth, watery texture and gentle floating motion (animated SVG turbulence + CSS).
- 🔊 **Soft, layered pop sounds** synthesized live with the Web Audio API — every pop is randomized in pitch, timbre, and timing, so no two sound alike.
- 💥 **Realistic pop animation** — burst, ripple ring, and splashing droplets, all synced to the sound.
- 🌐 **5 hidden golden-lattice spheres**, each a distinct color (gold, cyan, pink, green, violet), built as a Fibonacci sphere with golden-angle spiral lattice lines. Pop its bubble and the spinning 3D sphere pins itself exactly where the bubble burst.
- ⏱️ **60-second countdown** — a bold red timer that turns **bold and blinks** during the final 10 seconds.
- 🔁 **Living playfield** — every 10 seconds, 20 fresh bubbles are added, found spheres are re-hidden, and all 5 spheres reshuffle across the bubbles. Bubbles that drift off-screen are replaced, and their spheres hop to a random on-screen bubble.
- 🏆 **Win sequence** — find all 5 and every bubble bursts at once under a cascading watery splash, then **"YOU ARE THE WINNER!"** appears with the five spheres orbiting it.
- ⏳ **Time's Up sequence** — run out of time and the bubbles burst into a watery downpour with a **"TIME'S UP!"** message and a **Play Again** button.
- 📱 **Responsive & touch-friendly** — adapts bubble sizes, typography, and layout from phones to desktops.

---

## 🎮 How to Play

1. **Tap or click** any bubble to pop it.
2. Five bubbles hide a colored sphere — each gives off a faint colored glow as a hint.
3. **Pop all 5 sphere bubbles before the timer hits 0:00** to win.
4. The board refreshes every 10 seconds, so keep popping fast!
5. Hit **New Game** (top of screen) — or **Play Again** on the end screen — to start fresh.

> 💡 Sound unlocks on your **first tap** (browser autoplay policy), so the very first pop both pops *and* arms the audio.

---

## 🚀 Running Locally

No build, no dependencies to install. Either:

**Option A — just open it**
```bash
# clone, then open in a browser
git clone https://github.com/me-raffyrabin/bubblypop.git
cd BubblyPop
open index.html        # macOS  (use 'xdg-open' on Linux, or double-click on Windows)
```

**Option B — serve it (recommended)**
A local server avoids any browser file-access quirks:
```bash
# Python 3
python3 -m http.server 8000
# then visit http://localhost:8000
```

> ℹ️ The 3D spheres load **Three.js from a CDN (unpkg)**, so an internet connection is needed for that part. The bubbles and sounds work fully offline.

---

## 🌍 Deploy

It's a static site — host it anywhere:

- **GitHub Pages**: push to GitHub, then enable Pages on the `main` branch (root). Your game is live at `https://me-raffyrabin.github.io/bubblypop/`.
- Or drop the folder onto Netlify, Vercel, Cloudflare Pages, etc.

---

## 📁 Project Structure

```
BubblyPop/
├── index.html                  # the game (self-contained: HTML + CSS + JS)
├── golden-lattice-sphere.html  # standalone golden-ratio sphere visualizer (the spheres are based on this)
├── README.md
└── LICENSE
```

---

## 🛠️ Built With

- **Vanilla HTML / CSS / JavaScript** — no framework, no bundler.
- **Web Audio API** — real-time synthesized pop sounds.
- **SVG `feTurbulence` / `feDisplacementMap`** — the watery fluid texture inside each bubble.
- **[Three.js](https://threejs.org/) 0.160** (via CDN import map) — the animated golden-lattice spheres.
- **CSS animations & the Web Animations API** — bubble drift, bursts, splash, and the winner message.

---

## 🏷️ Topics

`game` · `bubble-pop` · `javascript` · `html5` · `threejs` · `web-audio-api` · `canvas` · `casual-game` · `vanilla-js` · `browser-game`

> Add these as your repo's GitHub **Topics** (the ⚙️ next to "About" on the repo page), or apply them all at once with the GitHub CLI:
>
> ```bash
> gh repo edit me-raffyrabin/bubblypop \
>   --add-topic game,bubble-pop,javascript,html5,threejs,web-audio-api,canvas,casual-game,vanilla-js,browser-game
> ```

---

## 📄 License

Released under the [MIT License](LICENSE). © 2026 extremeprogrammer.

---

<p align="center">Made with 🫧 and a love for popping things.</p>
