# Jetpack Rivals — real online multiplayer

Node.js WebSocket server. Players on different devices/networks join the same room via a room code or invite link. 2–4 players recommended; one player can test alone.

## Run locally

1. Install Node.js 18+.
2. In this folder run `npm install` then `npm start`.
3. Open http://localhost:3000 in a browser.

## Deploy for a public URL

Push this entire folder to a GitHub repository. Create a **Web Service** on Render.com linked to the repository, using build command `npm install` and start command `npm start`. Render will provide an HTTPS URL. Share that URL (or the in-game room invite link) with friends. Render free instances can spin down and disconnect players when idle; a paid always-on instance is better for stable matches.

**Important:** This multiplayer version needs a running Node.js server. Static-only hosting such as Netlify Drop or GitHub Pages will not support the multiplayer server.

Controls: Space / click / touch to fly; E or USE to activate collected item. The host starts the race. Banana jams an opponent's jetpack, knife slows an opponent, monkey slows the nearest player behind. First across the finish wins.

This is an early prototype. There is no account system, persistent matchmaking, anti-cheat, or automatic host migration during a race.
