# Hermann

Software engineering student in my last semester at Tec de Monterrey, based in Monterrey, Mexico. I mostly write TypeScript and Python, lately some Kotlin for Android, and I like the lower-level side too: audio, DSP, C and C++ when a project calls for it. Graduating December 2026 and available full-time from January 2027.

**CV:** [hermannpr.github.io](https://hermannpr.github.io/) ([English](https://hermannpr.github.io/cv/en-fullstack.html), [PDF](https://hermannpr.github.io/files/CV_Hermann_Pauwells_FullStack.pdf)) · [LinkedIn](https://www.linkedin.com/in/hermann-pauwells-rivera) · hermann.pauwells.rivera@gmail.com

<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" height="20" alt="TypeScript"> <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" height="20" alt="React"> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" height="20" alt="Next.js"> <img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white" height="20" alt="Node.js"> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" height="20" alt="Python"> <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" height="20" alt="Kotlin"> <img src="https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white" height="20" alt="Electron"> <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" height="20" alt="C++"> <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" height="20" alt="Supabase"> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" height="20" alt="PostgreSQL"> <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" height="20" alt="FastAPI"> <img src="https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white" height="20" alt="FFmpeg">

I'd rather build things people actually use than talk about what I could build. So far that's a real toy store's online shop, a reservations system with live occupancy, an original wavetable synth as a VST3, a 3DS synth in C, and three early-stage startups of my own.

## Startups

All three started in September 2026 and are early: working software, no users or revenue to report yet. Two of them are built on **[TypeSafe's Jev](https://openrouter.ai/typesafe)** (a decision model, via OpenRouter) for agent orchestration and explainable decisions.

- **HIVEMIND** (co-founder, private pilot): team chat for people and AI agents. Android (Kotlin/Jetpack Compose) and Windows (Electron) apps on a self-hosted ntfy server, HMAC-SHA256 signed messages, one-time beta invite codes and 104 automated tests on the Windows client.
  - **Agent orchestration with Jev:** a Python dispatcher (jev-lider) asks Jev which AI agent should take each message or task, under US$0.0001 per message with a US$0.50 daily cap, through our own Jev gateway running on an Android phone used as a server.
  - **Jev-guided context compaction** for long-running Claude Code bots: a fork of [fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction) (MIT) extended with a token budget, decay and a searchable archive so nothing is lost. On a real session it keeps ~57K tokens where the original kept ~229K, in 1.5 s.

  Private repo · [website](https://hivemind-web-rho.vercel.app) · [downloads](https://github.com/HermannPR/hivemind-chat-releases)

  [![HIVEMIND promo video (42 s)](https://hermannpr.github.io/files/hivemind-promo-poster.jpg)](https://hermannpr.github.io/files/hivemind-promo-720p.mp4)
  [Watch the 42 s promo video](https://hermannpr.github.io/files/hivemind-promo-720p.mp4)

  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" height="20" alt="Kotlin"> <img src="https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white" height="20" alt="Electron"> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" height="20" alt="Python">

- **Chécalo** (founder, in development): nutrition app for Mexico. Scan a barcode (Open Food Facts) and get the NOM-051 warning labels computed with deterministic rules checked against the DOF. **Jev** then gives an explainable verdict with its confidence and flags contradictions between ingredients and the nutrition table (every number still comes from the rules), behind a proxy with a per-product cache, so AI cost grows with the catalog and not with users. PWA plus an Android app (Kotlin, CameraX, ML Kit). Private repo.

  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" height="20" alt="Kotlin"> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" height="20" alt="JavaScript"> <img src="https://img.shields.io/badge/PWA-5A0FC8?style=flat-square&logo=pwa&logoColor=white" height="20" alt="PWA">

- **recaps-studio** (co-founder): a factory that turns a novel into a narrated, manhwa-style video. Resumable Python pipeline with a hash cache in SQLite: script, TTS with word-level timing (faster-whisper), shot planning, AI images checked by a vision judge, subtitles, and an FFmpeg/Remotion render. Human approval gates, a credit budget cap, automatic QA, and pytest with mocked providers. Private repo.

  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" height="20" alt="Python"> <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" height="20" alt="SQLite"> <img src="https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white" height="20" alt="FFmpeg"> <img src="https://img.shields.io/badge/Remotion-0B84F3?style=flat-square" height="20" alt="Remotion">

## Projects

- **[Juguetería El Arbolito](https://github.com/HermannPR/JugueteriaElArbolito)**: freelance client work. Online store and admin panel for a single-location toy store, in production: catalog, cart, checkout, Mercado Pago payments and an LLM chatbot. The 2,395-product catalog exported from the old point of sale is prepared for import, and the online/in-store inventory sync is in progress. [demo](https://jugueteria-el-arbolito.vercel.app)

  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" height="20" alt="Next.js"> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" height="20" alt="TypeScript"> <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" height="20" alt="Supabase"> <img src="https://img.shields.io/badge/Mercado_Pago-009EE3?style=flat-square" height="20" alt="Mercado Pago">

- **[folk-park](https://github.com/HermannPR/folk-park)**: original wavetable synth and composition assistant (VST3/Standalone, C++20/JUCE), with deterministic MIDI generation, automated test suites, and pluginval strictness 5.

  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" height="20" alt="C++"> <img src="https://img.shields.io/badge/JUCE-8D6E63?style=flat-square" height="20" alt="JUCE"> <img src="https://img.shields.io/badge/VST3-6A1B9A?style=flat-square" height="20" alt="VST3">

- **Lumina Reservations (WorkHub MTY)**: team project for office and parking reservations. I built the Node/Express reservations backend with live occupancy over SSE, and the React floor map and booking flow with role-based access. [demo](https://work-hub-mty-six.vercel.app/login)

  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" height="20" alt="TypeScript"> <img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white" height="20" alt="Node.js"> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" height="20" alt="Express"> <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" height="20" alt="Supabase">

- **HeatShield**: iOS app with real-time heat alerts, heat index and shelter maps. Won the Sustainability category at Swift Challenge Fest 2025 (Tec de Monterrey).

  <img src="https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white" height="20" alt="Swift">

- **Mildred Pierce**: transmedia website for my band: a channel-surfing experience with a CRT-TV look, chapters, a companion, leaderboards and fan uploads. [demo](https://mildred-pierce.vercel.app)

  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" height="20" alt="Next.js"> <img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" height="20" alt="Three.js"> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" height="20" alt="PostgreSQL">

### Smaller things

- [warehouse-model](https://github.com/HermannPR/warehouse-model): multi-agent Q-learning warehouse sim with a Unity visualization and a FastAPI backend
- [spectre-daw](https://github.com/HermannPR/spectre-daw): synth for the Nintendo 3DS, in C
- [PosturePRO](https://github.com/HermannPR/PosturePRO): pose estimation in the browser (MediaPipe)
- [JesusGPT](https://github.com/HermannPR/JesusGPT): AI Bible study app
- [forge](https://github.com/HermannPR/forge): personal dashboard
- [GateGenius](https://github.com/HermannPR/gategenius): AI airline-catering platform, built in 24 hours at HackMTY 2025
- **2HLABS**: preworkout brand site with a formula generator. [demo](https://2-hlabs.vercel.app)
- **laptop-deal-intelligence**: dashboard that scores laptop deals in Mexico. [demo](https://laptop-deal-intelligence.vercel.app)

## Open to

Junior / entry-level software engineering roles starting January 2027. Based in Monterrey; remote, hybrid or on-site all work. Strongest on full-stack TypeScript (React/Next.js, Node.js), comfortable with Python and Kotlin, and happy to go deep on audio, DSP or C/C++. If something here is useful to you, get in touch.

[Portfolio / CV](https://hermannpr.github.io/) · [LinkedIn](https://www.linkedin.com/in/hermann-pauwells-rivera) · [GitHub](https://github.com/HermannPR) · [Best works](https://hermannpr.github.io/best-works/)
