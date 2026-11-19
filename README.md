# Gullu English

Spelling games for a Year 1 student learning contractions (can't, don't, it's, I'm…).

Five games, in teaching order:

1. **Squish it**: two words squish into one and the apostrophe takes the place of the missing letters.
2. **Tap + Read**: tap each sound, then read the word.
3. **Tap + Zap**: tap the sounds, then zap (sweep) to blend them.
4. **Spell + Zap**: hear the word, spell it one sound per box, zap to check.
5. **Read + Spell**: look, say, cover, write, check.

There is also a parent guide and a Words page for choosing each week's list. Progress is saved in the browser.

## Project layout

```
public/index.html   the whole site (HTML, CSS and JS in one file)
wrangler.jsonc      Cloudflare Worker config (static assets only)
```

## Run locally

```bash
npm install
npm run dev
```

## Deploy to Cloudflare

```bash
npx wrangler login
npm run deploy
```

Wrangler uploads `public/` as static assets for a Worker named `gullu-english`, served at `gullu-english.<your-subdomain>.workers.dev`.
