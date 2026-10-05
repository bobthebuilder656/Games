# Arcade: Pixel Quest & Pinball

Two browser games, built entirely through conversation with Claude.

**Play: [games-pinballquest.netlify.app](https://games-pinballquest.netlify.app/)**

![Arcade landing page](docs/landing.png)

## The games

- **Pixel Quest** is a platformer with seven themed levels that end in a boss fight. It has six playable heroes, each with its own ability, plus collectible stars, power-ups and hidden secrets.
- **Pinball** has realistic flipper physics, ramps and multiball. It has six difficulty tiers from Rookie to Nightmare, five table themes, daily missions and a coin shop.

## Why it's different

- **No login.** There are no accounts, sign-ups or passwords.
- **No install.** It opens in any modern browser on a phone, tablet or laptop.
- **Safe and private.** The games don't collect any data and have no ads, trackers or analytics. They never contact another server. Progress and high scores are stored only in your own browser.
- **Free.** Nothing to buy. The in-game coin shop uses only coins you earn by playing.
- **Works offline.** Once a page has loaded, you can keep playing without an internet connection.
- **Built for mobile too.** Both games have on-screen touch controls and a fullscreen mode. Pixel Quest supports multi-touch, so you can move and jump at the same time.

## How it was built

- **Made with Claude.** Every line of code was written by Claude ([claude.ai](https://claude.ai)) through plain-language conversation: describe a feature, play it, give feedback, repeat.
- **One file per game.** Each game is a single self-contained HTML file. There are no frameworks, libraries, build tools or external assets. The graphics are drawn in code and the sound effects and music are generated in the browser.
- **Hosted on Netlify** as a static site, so there is no server or database behind it.
- **Automatically tested.** A Playwright test suite in `tests/` opens every page on desktop, phone portrait and phone landscape screen sizes. It checks for broken layouts, unreachable buttons, crashes and touch controls that fail when used together.

## Repo contents

| File | Purpose |
|---|---|
| `index.html` | Landing page |
| `platformer.html` | Pixel Quest |
| `pinball.html` | Pinball |
| `tests/` | Automated browser checks |
| `docs/` | README screenshot |

To run the games locally, download the repo and open `index.html`. To run the checks, run `npm install` and then `npm run check` inside `tests/` (requires Node.js).
