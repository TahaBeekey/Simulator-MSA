# Simulator MSA

Reel order and price simulator for MSA GROUP CONDOR (AI Instagram reels).

A single file, `index.html`: HTML, CSS and vanilla JavaScript, with no build step and no backend. It opens directly in a browser and deploys as is on Vercel or any static host.

## What it does

- Builds an order à la carte (100 % IA, B-roll and voix off reels, at least 2 reels) or a monthly pack (6, 8 or 10 reels).
- Shows the exact price as you go: reels subtotal, maintenance, "Total du mois", Voiceflow shown separately, and a total that includes it.
- Sends the request on WhatsApp with a prefilled message, prints a one-page summary, and opens the brief form ("Remplir les briefs").

No data is stored or sent anywhere. The current setup is only kept in the part of the page address after `#`.

## Editing prices

All prices are in the `CONFIG` object at the top of the script in `index.html`. Change a number there, and the page, the summary and the WhatsApp message all follow.

## Link options

- `?client=…&commande=…` is passed to the brief form (default client: `MSA`).

## Tests

Open `index.html?test=1`. The results show at the bottom of the page and in the browser console.
