# Farcaster Coinflip Miniapp

Two-chain coinflip:
- Flip on **Arbitrum** (Heads = instant reward on Arbitrum, Tails = claim on Base)
- Claim on **Base**
- Leaderboard reads top 10 total flips from Arbitrum

## Quick start

1. Put your images:
   - `public/arbitrum.png`
   - `public/base.png`

2. Verify contract JSONs:
   - `public/arbitrumGame.json` (address + ABI)
   - `public/baseClaim.json` (address + ABI)

3. Serve locally:
   - Use any static server, e.g.:
     ```bash
     npx http-server -p 5173 .
     ```
   - Open `http://localhost:5173`

4. Deploy:
   - **Vercel** or **GitHub Pages** (static hosting)

## Notes
- Uses wagmi + Farcaster Miniapp connector (esm.sh) — no Node build needed.
- Toast popups are modern, glassmorphism style.
- Change reward images/branding in `index.html` as you like.
