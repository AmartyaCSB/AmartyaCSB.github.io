---
layout: post
title: "Avalon Voice Agent"
description: A browser-based voice host for The Resistance: Avalon with advanced Big Box roles, validation, and optional premium TTS.
tags: [avalon, games, web, typescript, react, vite, tts, node, express]
categories: projects
---

**Intro**: I built a voice agent that narrates the Avalon setup reveal stage with configurable roles along with advanced roles of Avalon Bigbox, speed controls, repeats, and seat validation. It runs fully in the browser with a server option for premium Text to Speech (TTS)

### Why
I love playing Avalon with my close friends in Atlanta and wanted a zero-rule-lookup. I'm planning to build a discord style integration and a web-app for **host** that helps new players along with advanced Big Box variants because I haven't seen any website as such which does these both. Lots of development to follow on this! I also wanted to learn Typescript and React!

### What it does
- Pick players (5–10), toggle base & advanced roles, auto-validate seats, and **narrates** the reveal script.
- Live **speed** and **repeat** controls; one-click **Stop/Restart**.
- Optional advanced modules (Lancelots, Messengers, Rogues/Sorcerers, Lady of the Lake, etc.) and checks validation.
- Works offline with Web Speech API; optionally uses a small server for ElevenLabs-style TTS.

### Stack
- **Client**: React + TypeScript + Vite, Web Speech API (browser TTS).
- **Server (optional)**: Node + Express + ts-node, streaming MP3 TTS with caching.
- **Deploy**: GitHub Pages 

### Challenges & fixes
- **Subpath on GitHub Pages**: assets & fetches broke; fixed by reading `BASE_URL` for routes and `rules.md`.
- **Stop/restart TTS cleanly**: added a `runRef` token and `Audio`/speechSynthesis cancel to avoid stuck states.
- **Role validity**: real-time checks (Good/Evil seat math, Oberon/Mordred/Morgana rules) with clear alerts.
- **Playback UX**: per-line TTS and for repeat N times, small gaps in speech, and a cache to avoid refetching audio.

### Follow, play and have fun!
- **Repo**: <https://github.com/AmartyaCSB/avalon-voice-agent>  
- **Live demo** : [`/Avalon Voice Agent/`  ](https://amartyacsb.github.io/avalon-voice-agent/)


