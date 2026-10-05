# 🏎️ Endless Highway Racer

An endless 3D traffic-racing game that runs right in your browser. Dodge traffic, grab coins, chain near-misses for combos, and unlock new vehicles, maps and upgrades. Built with **Three.js**, with a mobile-first touch / tilt control scheme.

**Developer:** Tarun Saini

---

## ✨ Features

- **Endless highway gameplay**: speed ramps up the longer you survive
- **Near-miss combo system** (up to x5) that gives bonus score and refills nitro
- **Nitro boost** with a refilling meter
- **5 vehicles**: Sedan, Sports Bike, Heavy Truck, Cycle, Lamborghini
- **8 maps**: Autumn Highway, Desert, Snow, City Night, Village, Mountain Ghat, Coastal Highway, Storm Rain
- **Dynamic world**: day/night, rain, sandstorms, tunnels and bridges
- **Mixed traffic**: cars, buses, rickshaws, tempos and bikes
- **Garage and abilities**: buy vehicles and upgrade Nitro Power, Nitro Tank, Recharge, Grip and Shield
- **Realistic crashes**: slow-motion tumble, sparks and cracked glass
- **Wheelie** mode on the bike, working horn, indicators and a live gear/RPM cluster
- **In-game music player** with 5 tracks
- **Scoreboard** (top 10 runs) and progress saved in `localStorage`
- **Settings**: graphics (low / med / high), volume, km/h or mph, camera shake, time of day, weather, auto/manual speed mode

---

## 🎮 Controls

### Keyboard

| Action | Keys |
|---|---|
| Steer | `A` / `D` or `←` / `→` |
| Brake | `S`, `↓` or `Space` |
| Nitro | `Shift` or `N` |
| Wheelie (bike) | `W` or `↑` |
| Horn | `H` |
| Indicators | `Q` (left) / `E` (right) |
| Pause / Resume | `Esc` or `P` |
| Start | `Enter` |

### Mobile

- **Touch**: on-screen steer, brake, nitro and wheelie buttons
- **Phone rotate (tilt)**: switch under *Settings → Controls*, then use *Calibrate* to set your neutral angle

---

## 🚀 Getting Started

### Project structure

```
highway racer/
├── index.html     # Game (HTML + CSS + JS)
├── three.min.js   # Three.js library
├── songs.json     # Music playlist
└── song1.mp3 … song5.mp3
```

### Run locally

The game loads `songs.json` and the music files, so serve it over HTTP instead of opening the file directly.

```bash
# Python
cd "highway racer"
python3 -m http.server 8000

# or Node
npx serve .
```

Then open **http://localhost:8000** in your browser.

### Deploy

It is a static site with no build step. Upload the folder to any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages, etc.).

---

## 🎵 Customizing the Music

Edit `songs.json` to change the playlist:

```json
[
  { "file": "song1.mp3", "name": "Legendary 1" },
  { "file": "song2.mp3", "name": "Legendary 2" }
]
```

Put your MP3 files next to `index.html` and list them here.

---

## 🛠️ Tech Stack

- HTML5, CSS3, vanilla JavaScript
- [Three.js](https://threejs.org/) for WebGL rendering
- Web Audio API for engine, horn and effect sounds
- Device Orientation API for tilt steering

---

## 🌐 Browser Support

Any modern browser with WebGL: Chrome, Edge, Firefox, Safari (desktop and mobile). Tilt controls need a device with motion sensors, and iOS asks for motion permission.

---

## 📄 License

The source code is released under the [MIT License](LICENSE).

- Three.js is also MIT licensed (© three.js authors).
- Audio files are **not** covered by the MIT License. Make sure you have the rights to any music you include or distribute.

---

## 👤 Author

**Tarun Saini**

If you enjoy the game, give the repo a ⭐ and share your high score!
