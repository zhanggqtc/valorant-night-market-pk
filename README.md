# VALORANT · 夜市皮肤 PK 大作战

A static, single-file interactive demo: spin the VALORANT Night Market for 6 random skins, then duel an AI rival in a 3-round "best-of-three" tactical match — inspired by the classic Chinese strategy *Tian Ji's Horse Race*.

> **Live demo**: https://zhanggqtc.github.io/valorant-night-market-pk/
>
> **在线预览**：https://zhanggqtc.github.io/valorant-night-market-pk/

---

## ✨ Features

- **6-Slot Night Market**: Random rolls across 5 tiers (Select / Deluxe / Premium / Exclusive / Ultra) with discount %, wishlist score, weapon SVG art, and combat-power calculation.
- **Tian Ji's Horse-Race Strategy**: Pick 3 skins for battle. The system auto-grades them as upper / middle / lower horse. Choose your deployment order (1st, 2nd, 3rd slot) to outsmart the AI rival.
- **Best-of-3 Battle**: Real-time duel animation, round-by-round result indicators, full battle log.
- **Sharable Win Card**: After victory, generate a 720×1080 canvas poster and download to share — opponent's lineup is hidden so they can't guess your strategy.
- **Persistent Stats**: LocalStorage-backed match history, 5-win streak unlocks a reward badge.
- **Pure Static**: One single `index.html` file, ~110 KB. No build step, no backend. Drop it on any web server.

## 🎮 How to Play

1. **Stage 1 — My Night Market**: 6 random skins are auto-revealed. Click 「重新抽取夜市」 (Reroll) for a different draw.
2. **Stage 2 — Tactical Lineup**: Pick 3 of the 6 skins. The system labels them upper/mid/lower horse by combat power. Drag-and-drop into 1st / 2nd / 3rd slot — order matters!
3. **Stage 3 — Battle**: AI rival reveals their 3 skins one round at a time. Best of 3 wins.
4. **Stage 4 — Result**: Win → unlock a sharable poster + counter towards 5-win reward. Lose → review battle log and try again.

## 🛠 Tech

- Vanilla HTML / CSS / JS — zero dependencies bundled into one file
- External CDN: [RemixIcon](https://remixicon.com/) (icons), [QRCode.js](https://github.com/davidshimjs/qrcodejs) (share QR)
- Inlined: 11 weapon SVGs, full skin database, view/data/main modules

## 📁 Project Structure

```
valorant-night-market-pk/
├── index.html      # Single-file demo (CSS + JS inlined)
└── README.md
```

## 🚀 Deploy Anywhere

Since it's a single static file, just serve it:

```bash
# Local preview
python3 -m http.server 8080
# then open http://localhost:8080
```

Or drop `index.html` on any static host (GitHub Pages / Netlify / Cloudflare Pages / S3 / nginx).

## 📜 License

MIT — see [LICENSE](./LICENSE).

> This is an unofficial fan-made interactive demo. **VALORANT** and all related artwork, names, and trademarks are property of Riot Games, Inc. This project is not affiliated with or endorsed by Riot Games.
