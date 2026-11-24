# WORLD LOGISTICS EMPIRE — Playable Prototype 0.1

A mobile-first, browser-playable vertical slice of the global logistics tycoon concept.

## Run locally
Open `index.html` in a modern browser. No build tools or internet connection are required. Progress is saved in the browser's local storage.

## Install on a phone (PWA)
When these files are hosted on an HTTPS domain, open the site in Safari on iPhone and use **Share → Add to Home Screen**. On Android, use the browser's **Install app** option. The service worker caches the game shell for offline reopening. The actual world simulation in this prototype runs in the browser; it is not a persistent shared server simulation.

## Included gameplay
- Global schematic world map and route visualization
- Four transport modes: road, rail, air, sea
- Dynamic cargo offer board
- Fleet purchases, capacity and availability
- Contract acceptance and dispatch
- Operating costs, revenue, profit, reputation
- Automatic shipment progress and offline catch-up based on timestamps
- Local save game

## Prototype limitations
This is a playable single-device prototype, not the public multiplayer release. It has no account system, cloud saves, server-authoritative economy, real map tiles, live market, payments, anti-cheat, or App Store / Google Play packaging. The world map is schematic. All simulation values are prototype balancing values.

## Production direction
The production stack remains Unity (iOS/Android client) + ASP.NET Core server + PostgreSQL/PostGIS, with Redis/SignalR where justified. The next release gate is a server-authoritative online backend, followed by the production 3D globe/client, QA, hosting, store accounts, signing, and app-store submission.
