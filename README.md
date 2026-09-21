# Nexora — Crypto Platform Website

A modern, dark-themed cryptocurrency platform website built with plain **HTML, CSS and JavaScript**, all in a single `index.html` file. No frameworks, no build step, no image files.

**Created by Jagdish Maliwad**

---

## Preview

The page includes:

- Sticky navigation with dropdown menus, Log In and Sign Up buttons
- Hero section with a tilted phone mockup, 3D-style Bitcoin and Ethereum coins and a glowing platform
- Live price ticker (BTC, ETH, SOL, BNB, XRP, ADA)
- "Everything You Need in One Crypto Platform" feature cards
- Market Overview with Top Gainers, Top Losers and Most Active tabs
- "Start Your Crypto Journey Today" call-to-action card
- Animated stats row (users, coins, volume, uptime)
- Newsletter subscription box
- Full footer with links, social icons and app download buttons

---

## Getting Started

1. Download `index.html`.
2. Double-click it to open in any modern browser (Chrome, Edge, Firefox, Safari).

That's it. To host it, upload the file to any static host such as GitHub Pages, Netlify or Vercel.

> An internet connection is only needed for the Google Fonts (Inter and Michroma). Without it, the page falls back to system fonts.

---

## Interactive Features

| Feature | What it does |
|---|---|
| Live price ticker | Prices move every second or so with a green or red flash. The ticker, phone watchlist and market list stay in sync. |
| Phone portfolio | The balance, 24h change and chart update with the prices. |
| Market tabs | Switch between Top Gainers, Top Losers and Most Active. |
| Quick trade | Click any coin, Buy, Sell or Trade to open a trade window with fee and quantity calculations. |
| Log In / Sign Up | Form validation, then the nav switches to a user avatar and Log out button. |
| Newsletter | Email validation with a confirmation message. |
| Stats | Numbers count up when scrolled into view. |
| Responsive layout | Works on desktop, tablet and mobile, with a hamburger menu on small screens. |
| Accessibility | Keyboard focus styles, ARIA labels and reduced-motion support. |

---

## Live Market Data (Optional)

By default the site shows the prices from the original design and simulates small live movements.

To use real prices from the public CoinGecko API, open `index.html`, find this line near the top of the `<script>` section and change it:

```js
const USE_LIVE_DATA = false;   // change to true
```

Prices then refresh every 60 seconds. If the API is unavailable, the site falls back to the simulated feed. The free CoinGecko API is rate-limited, so avoid very frequent refreshes.

---

## Demo Mode Notice

This is a front-end demo. **Nothing is sent to a server or stored.**

- Log In and Sign Up are simulated.
- Trades are simulated and no real funds move.
- Footer and dropdown pages (Careers, Terms, etc.) show a "not part of this demo" message.

To turn it into a real product, connect the forms and trade button to your own backend and authentication service.

---

## Customising

- **Colors:** edit the CSS variables in the `:root` block at the top of the `<style>` section (`--purple`, `--green`, `--bg`, and so on).
- **Coins and prices:** edit the `COINS` object in the script. Each entry has a name, price, 24h change and volume.
- **Coin icons:** the `ICONS` object holds the inline SVG for each coin. Coins without an entry get an automatic letter icon.
- **Text and links:** edit the HTML directly. Links marked `data-soon` show the demo message. Replace them with real URLs when your pages exist.
- **Brand name:** search for "Nexora" and replace it, and update the logo SVG if needed.

---

## Project Structure

```
index.html   # everything: markup, styles and scripts
README.md    # this file
```

---

## Browser Support

Latest versions of Chrome, Edge, Firefox and Safari. The trade and login windows use the native `<dialog>` element.

---

## Disclaimer

Nexora is a fictional brand and this project is a design and front-end demonstration. It is not financial software. Cryptocurrency trading carries risk, so do your own research before investing.

---

## Author

**Jagdish Maliwad**
