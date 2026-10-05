# Arcade: Pixel Quest & Pinball

Two free browser games. You don't need to install anything, and they work on a phone or a laptop.

**▶ Play now: [games-pinballquest.netlify.app](https://games-pinballquest.netlify.app/)**

Your progress and high scores are saved in your own browser. There are no accounts and no ads.

---

## 🟩 Pixel Quest (platformer)

A pixel-art platformer with seven themed levels that end in a boss fight against **The Goober King**.

- **Levels:** Green Hills → Broken Bridge → Desert Ruins → Crystal Caves → Frozen Peaks → Haunted Forest → The Goober King
- **Six heroes, each with an ability:** Bolt (balanced), Tank (extra life), Pip (tiny and nimble), Rosie (higher jump), Gizmo (fast runner), Nova (floaty falls). You unlock Rosie, Gizmo and Nova by clearing the early levels.
- **Three stars per level:** one for reaching the flag, one for collecting every coin and one for finishing without losing a life
- **Power-ups:** shield, extra life, speed boost, super jump, coin magnet, fireball
- **Secrets** in every level. Some spots can only be reached by one particular hero.
- **Trophy case** with goals that span the whole game

**Controls**

| Action | Keyboard | Touch |
|---|---|---|
| Move | ← → or A / D | On-screen arrows |
| Jump (press again in the air to double jump) | ↑, W or Space | Jump button |
| Duck | ↓ or S | Duck button |

Best on a desktop. On a phone, turn it sideways (landscape).

## 🩷 Pinball

A pinball table with realistic flipper physics, ramps, combos and multiball.

- **Difficulty tiers:** Rookie → Pro → Expert → Master → Insane → Nightmare (plus a secret Legendary tier). Each new tier repaints the table and adds more bumpers, spinners and targets.
- **Five table themes:** Ocean Rush, Neon City, Lost Temple, Haunted Carnival and Space Odyssey. Each one has its own special mode.
- **Daily challenge and daily missions**
- **Shop:** spend the coins you earn on perks (Steady Grip, Safety Net, Head Start, Legendary Tier) or on one-use items (Extra Ball, Mission Reroll)
- **Achievements**, skill shots, and nudging the table (nudge too hard and it tilts)

**Controls**

| Action | Keyboard | Touch |
|---|---|---|
| Launch the ball | Hold Space, then let go | Launch button |
| Left flipper | Z or ← | Left side |
| Right flipper | / or → | Right side |
| Nudge | X or ↓ | Nudge button |

Works well on both desktop and mobile.

---

## What's in this repo

| File | What it is |
|---|---|
| `index.html` | The arcade home page, where you pick a game or press **Surprise Me** |
| `platformer.html` | Pixel Quest |
| `pinball.html` | Pinball |
| `tests/` | An automated check that opens every page on desktop and phone screen sizes and reports anything broken |

Each game is a single HTML file with no external libraries. To play offline, download the repo and open `index.html` in any browser.

### Running the checks (optional)

You need [Node.js](https://nodejs.org/) installed. Then run:

```bash
cd tests
npm install
npx playwright install chromium
npm run check
```

To check the live site instead of your local files, set `BASE_URL=https://games-pinballquest.netlify.app` before running `npm run check`.

---

Made with [Claude](https://claude.ai).
