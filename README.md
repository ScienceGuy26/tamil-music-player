# Tamil Music Player

> A Tamil-first open-source web music player with a built-in ringtone maker.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Why This Exists

Existing open-source music players treat Tamil music as an afterthought. This project is a Tamil-first player with proper Tamil typography, discovery by composer and film, and a built-in ringtone maker — all with legally clean streaming.

## Architecture

Client-only design. Audio streams from legally permissible APIs (currently Jamendo) and is never hosted by this app. The ringtone maker runs entirely in the browser using the Web Audio API.

App → Provider Abstraction Layer → [Jamendo, Internet Archive, YouTube Embed]


## Tech Stack

Next.js 16 · TypeScript · Tailwind CSS · Zustand · Howler.js · Supabase

## Roadmap

- [x] Scaffold and environment
- [x] Jamendo integration
- [ ] Search and playback
- [ ] Ringtone maker
- [ ] User accounts and playlists
- [ ] Deployment

## Legal Compliance

- Streams only CC-licensed and public domain content
- No server-side hosting of copyrighted audio
- Ringtone maker operates entirely client-side
- Not affiliated with any streaming service, label, or rights organization
- Music provided by [Jamendo](https://www.jamendo.com) under Creative Commons licenses

## Getting Started

```bash
git clone https://github.com/ScienceGuy26/tamil-music-player.git
cd tamil-music-player
npm install
cp .env.example .env.local   # add your Jamendo Client ID
npm run dev

Contributing
Contributions welcome. Open an issue first to discuss changes.

License
This project is licensed under the MIT License. See LICENSE for details.