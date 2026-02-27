# 🌍 Earth's Last Stand
### Epic Sci-Fi Tower Defense Game — PWA Ready

![License](https://img.shields.io/badge/license-MIT-blue)
![PWA](https://img.shields.io/badge/PWA-ready-brightgreen)
![Deploy](https://img.shields.io/badge/deploy-Vercel-black)

A fully-featured browser tower defense game built with HTML5 Canvas. No frameworks, no dependencies — pure JavaScript. Deploy anywhere, install as a PWA, play offline.

## 🎮 Features

- **15 Waves** of escalating alien invasions + **Endless Mode**
- **5 Tower Types** — each with 3 upgrade levels
  - 🔫 Vulcan Turret — rapid fire, great vs swarms
  - ⚡ Tesla Coil — chain lightning between enemies
  - 🚀 Rocket Battery — massive AoE splash damage
  - ❄️ Cryo Cannon — slows and freezes enemies
  - 🔬 Laser Beam — armor-piercing continuous beam
- **10 Enemy Types** with unique mechanics
  - Splitters, Bombers, Regenerators, Flying units, Bosses
- **3 Power-ups** — Cryo Freeze, Airstrike, Emergency Repair
- **Speed control** — 1x, 2x, 3x game speed
- **Particle effects**, screen shake, floating damage numbers
- **Keyboard shortcuts** — [1-5] towers, [Space] wave, [Esc] deselect
- **Fully responsive** — desktop & mobile

## 🚀 Deploy to Vercel (2 minutes)

### Option A — Vercel CLI
```bash
npm i -g vercel
vercel
```

### Option B — GitHub + Vercel Dashboard
1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import your GitHub repo
4. Click **Deploy** — done!

### Option C — Drag & Drop
1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag the project folder onto the page
3. Done!

## 📱 PWA Installation

After deployment, players can install the game as a native app:
- **Chrome/Edge**: Click the install icon in the address bar
- **iOS Safari**: Share → Add to Home Screen
- **Android**: "Add to Home Screen" prompt appears automatically

## 🗂️ File Structure

```
earths-last-stand/
├── index.html          # Complete game (single file)
├── manifest.json       # PWA manifest
├── sw.js               # Service worker (offline support)
├── vercel.json         # Vercel deployment config
├── icons/
│   ├── icon.svg        # Master icon
│   ├── icon-192.png    # PWA icon (generate from SVG)
│   └── icon-512.png    # PWA icon large (generate from SVG)
└── README.md
```

## 🎨 Generating Icons

Convert `icons/icon.svg` to PNG for full PWA support:

```bash
# Using ImageMagick
convert -resize 192x192 icons/icon.svg icons/icon-192.png
convert -resize 512x512 icons/icon.svg icons/icon-512.png

# Or use online: https://cloudconvert.com/svg-to-png
```

## 🛠️ Local Development

No build step needed — just open the file:

```bash
# Python
python -m http.server 8080

# Node
npx serve .

# Then open: http://localhost:8080
```

> ⚠️ Must serve via HTTP (not file://) for Service Worker and fonts to work.

## 🎯 Gameplay Tips

- Place **Cryo Cannons** next to damage towers for combo bonus
- **Tesla Coils** are best placed where enemies cluster/turn
- Save **Power-ups** for Boss waves (every 10 waves)
- **Sell** underperforming towers and rebuild as you learn the path
- **Rocket Batteries** are devastating in chokepoints
- Upgrade towers to Level 3 before buying new ones

## 📈 Roadmap

- [ ] Leaderboard (Supabase integration)
- [ ] 3 additional maps
- [ ] Sound effects & music
- [ ] Mobile touch controls optimization
- [ ] Tower synergy visual indicators
- [ ] Daily challenge mode
- [ ] Achievement system

## 📄 License

MIT — free to use, modify, and deploy.

---

Built with ❤️ — pure HTML5, no frameworks, no build tools needed.
