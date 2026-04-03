# GLOBAL BUG - WhatsApp Bot

## Overview
A WhatsApp bot built on the Baileys library (Node.js). It provides automation, group management, media downloading, AI chatbot features, and more.

- **Version:** 9.5.0
- **Author:** GlobalTechInfo (Qasim Ali)
- **Entry Point:** `index.js` (obfuscated)

## Tech Stack
- **Runtime:** Node.js 20
- **Package Manager:** npm
- **WhatsApp Library:** `@whiskeysockets/baileys` (aliased as `@adiwajshing/baileys`)
- **Database:** LowDB (local JSON) + MongoDB (optional via mongoose)

## Project Structure
- `index.js` — Main entry point (obfuscated); handles WhatsApp connection and auth
- `painzy.js` — Message handler and command logic
- `config.js` — Global bot configuration (owner numbers, bot name, etc.)
- `lib/` — Utility modules (myfunc.js, simple.js, premium.js, lowdb/, etc.)
- `database/` — JSON files for persistent data (limits, premium users, etc.)
- `session/` — WhatsApp auth credentials (creds.json)
- `GlobalMedia/` — Media assets for bot responses
- `image/` — Static images used by bot

## Running the Bot
```
npm start
```
The bot runs as a console process (no web frontend). On first run, it may prompt for an access code as part of the obfuscated licensing system.

## Workflow
- **"Start application"** — `npm start` (console output)

## Notes
- The `index.js` is heavily obfuscated to protect connection logic.
- On startup the bot prompts for an access code ("Kode Akses") — this is part of the licensing system.
- WhatsApp session credentials are stored in the `session/` directory.
