<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://yaleedhaque.github.io/banner.svg">
  <img alt="Md. Yaleed Haque — C#/.NET and Kotlin engineer, Dhaka, Bangladesh. 295 desktop commands, 27,800 lines of TypeScript, 486 automated tests."
       src="https://yaleedhaque.github.io/banner-light.svg" width="960">
</picture>

<h1 align="center">
  <strong style="font-size:1.25rem">Md. Yaleed Haque</strong>
  <br>
  <em>Systems engineer building offline-first software — C#/.NET, Kotlin/Android, TypeScript.</em>
</h1>

<p align="center">
  <a href="https://yaleedhaque.github.io"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-yaleedhaque.github.io-181717?logo=github&logoColor=white"></a>
  <a href="#proof"><img alt="Evidence" src="https://img.shields.io/badge/Verified%20with%20tests%20%2B%20CI-2ea44f"></a>
  <img alt="Open to work" src="https://img.shields.io/badge/Open%20to%20work-remote%20available-00e676">
  <a href="#contact"><img alt="Email" src="https://img.shields.io/badge/Email-contact%20me-blue?logo=gmail&logoColor=white"></a>
</p>

<p align="center">
  <img alt="C# .NET 8" src="https://img.shields.io/badge/C%23-.NET%208-512BD4?logo=csharp&logoColor=white">
  <img alt="Kotlin" src="https://img.shields.io/badge/Kotlin-Jetpack%20Compose-7F52FF?logo=kotlin&logoColor=white">
  <img alt="Android" src="https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white">
</p>

---

## The short version

I'm a systems engineer who ships complete products end to end — not toy demos. **30 repositories, MIT/Apache-2.0 licensed, most with CI and automated test suites.** My work runs where the constraints are real: sub-5 ms input latency, Bluetooth stacks, low-level Windows APIs, and databases with row-level security.

**What I'm looking for:** a full-time role doing **C#/.NET desktop work, Android/Kotlin work, or AI-agent/automation tooling** — ideally remote-friendly or Dhaka-based.

---

## Proof, not claims

Numbers I can show you, and where to check them:

| What | Evidence |
|---|---|
| **295-command desktop automation API** | `StarkAgent` → `Core/CommandCatalog.cs` — 295 registered actions |
| **~15,500 lines of production C#** | StarkAgent, OCR + UIA + Vision + CDP + DirectX capture |
| **~27,800 lines of TypeScript** | Family Tapestry — Next.js, React Flow, Supabase, Leaflet |
| **239 automated tests** | Family Tapestry, on 16 test files, Vitest — `src/lib/__tests__/`, `src/components/__tests__/` |
| **347 tests across 22 files** | AI Browser Toolkit, Python — drives a real Chrome/Edge over CDP |
| **7 database migrations** | Family Tapestry `supabase/` — `schema.sql` + `migration-v2…v7`, RLS enabled |
| **CI on 9 repos** | GitHub Actions — build, test, and release pipelines |

I write tests because the work is concurrency- and latency-sensitive, not because a checklist said so.

---

## Selected work

> **Note on access:** most source is private by default, marked `private` below — the code is available on request and I can walk through the architecture live. Every project that is live or downloadable links straight to the product; the few public repos are open to review now.

### Desktop automation & AI agents
- **[StarkAgent](https://github.com/yaleedhaque/StarkAgent)** — Fully autonomous Windows desktop control agent. **295+ commands** across mouse, keyboard, OCR, UIA tree-walking, file operations, web fetch, and email, over a local TCP/JSON API. Includes a WhatsApp driver and MCP server. *(C# · 15.5k LOC · MIT)*
- **yale-agent** `private` — Wayland-native Linux desktop agent: **68 tools** in 11 categories (vision click-by-text, browser, desktop, media, audio, filesystem, system) via MCP server, CLI, and web dashboard. *(Python)*
- **[AI Browser Toolkit](https://github.com/yaleedhaque/Ai-Browser-Toolkit)** — Let an AI agent drive real Chrome or Edge over a JSON API. One server, one persistent profile, full DOM control. **347 tests.** *(Python · Apache-2.0)*
- **precise-hands** `private` — Exact-coordinate MCP eye+hand: AT-SPI / XDG portal for Linux, uiautomator bounds → `input tap` for Android. *(Python)*
- **NetSpeedBar** `private` — Always-on-top taskbar network overlay with single named-mutex instance handling. *(C#)*
  **Download:** <https://yaleedhaque.github.io/downloads/files/NetSpeedBar.exe>

### Android / Kotlin
- **NovaCalc** `private` — Scientific calculator: fx-991-style keypad, function graphing, equation solver, QR read & generate, and a periodic table. No ads, no tracking, zero cloud. *(Kotlin + Compose)*
  **Download:** <https://yaleedhaque.github.io/downloads/files/NovaCalc-v1.1.0.apk>
- **Lumen** `private` — Offline torch: LED, screen light, strobe, SOS, Morse send, and **Morse decode from the camera** via ML Kit. *(Kotlin + Compose)*
  **Download:** <https://yaleedhaque.github.io/downloads/files/Lumen-v1.2.1.apk>
- **AetherCompass** `private` — Feature-packed offline compass with accurate bearings. *(Kotlin + Compose)*
  **Download:** <https://yaleedhaque.github.io/downloads/files/AetherCompass-v1.2.0.apk> · **offline maps & routing packs:** <https://github.com/yaleedhaque/aether-maps-packs/releases/tag/maps-packs>
- **BluetoothRemoteHid** `private` — Turn a phone into a wireless keyboard, touchpad, air-mouse and media remote for any PC over **Bluetooth Classic + LE HID**. No host software, no cloud. *(Kotlin)*
  **Download:** <https://yaleedhaque.github.io/downloads/files/BluetoothRemoteHid-v1.2.6.apk>
- **GamePadEcosystem** `private` — Android phones as wireless Xbox 360 controllers. **Sub-5 ms latency**, offline multiplayer, zero cloud. *(C# host + Kotlin)*
  **Download:** <https://yaleedhaque.github.io/downloads/files/GamePad-v1.2.0.apk>
- **OmniFetch-Android** `private` — On-device video search, stream and download with a bundled yt-dlp + ffmpeg engine. *(Kotlin + Compose)*
  **Download:** <https://yaleedhaque.github.io/downloads/files/OmniFetch-Android-v1.2.5-arm64.apk>

### Web & product
- **Family Tapestry** `private` — Collaborative graph-based family tree: real-time presence, timeline, map, generations, sub-tree collapse, multi-format export. Next.js + TypeScript + Supabase (RLS) + React Flow + Leaflet. **239 tests, 27.8k LOC, 7 migrations.**
  **Live site:** <https://family-tapestry-nine.vercel.app>
- **bKash + WhatsApp Storefront** `private` — Sellable e-commerce template for Bangladeshi local shops: manual bKash payment, WhatsApp order flow, stock, categories, admin dashboard.
  **Live site:** <https://bkash-ecommerce.vercel.app>
- **KhabarBD** `private` — A free, community-first food & drink atlas of Bangladesh: **18,177 places across 5,919 admin regions**, dish-level rankings, reviews, XP and badges. Next.js + Supabase (auth + row-level security) with **roles** (owner / admin / editor / user) and a moderation dashboard.
  **Live site:** <https://khabar-bd.vercel.app>
- **ঘুরে রাঙাও (Ghure Rangaao)** `private` — Offline-first Bengali travel planner: explore where to go, discover hidden gems, plan a trip, and collect a shareable travel passport. All in the browser.  <https://ghure.vercel.app>
  **Live site:** <https://yaleedhaque.github.io/downloads/sites/ghure-rangaao/>
- **Thikana (ঠিকানা)** `private` — Offline-first Bangladeshi rent & mess finder. *(private beta)*
- **ProctorFree** `private` — Browser-based exam proctoring; all AI runs client-side — no servers, no tracking, no accounts.
  **Live app:** <https://yaleedhaque.github.io/downloads/sites/proctorfree/>
- **YaleDoc** `private` — Self-encrypting documents in **one HTML file**. AES-256-GCM, PBKDF2-SHA256, encrypted version history, attachments, English/বাংলা UI, opens offline anywhere.
  **Download:** <https://yaleedhaque.github.io/downloads/files/YaleDoc-Blank.ydoc.html>
- **Haque Code** `private` — Offline universal barcode suite, plus the *Haque Vision* plugin (photo-in-QR, auto-open, recreate) and an Android wrapper. *(HTML + Kotlin)*

### Systems & networking
- **[YaleVPN-PC](https://github.com/yaleedhaque/YaleVPN-PC)** — Desktop WireGuard + Cloudflare WARP client for Linux and Windows: on-device keys, egress IP rotation, kill switch, DNS pinning, GUI + CLI. *(Python)*
- **[yalevpn](https://github.com/yaleedhaque/yalevpn)** — WireGuard VPN + Shizuku integration research lab for Android. *(Kotlin)*
- **stark-hotspot** `private` — Run a WiFi hotspot while staying connected to WiFi: concurrent STA+AP on one radio (hostapd + dnsmasq + NAT). *(Shell)*
- **Edge** `private` — Self-hosted on-device speech-to-text. Word-timed transcripts with clickable words, txt/srt/vtt export, faster-whisper + ffmpeg. No cloud, no API keys. *(Python)*

### Games
- **haque-squad** `private` — Authoritative-server multiplayer arena shooter (Godot 4) with phone browser touch controllers over WebSocket. 13 weapons, 5 maps, FFA/TDM/COOP, bots. *(GDScript)*

### AI tooling & agent infrastructure
- **opencode-dotfiles** `private` — Version-controlled AI agent brain: config, scripts, skills, memory, research, systemd units. Secrets handled through an encrypted vault with one passphrase held outside the repo.
- **opencode-setup-kit** `private` · **opencode-free-fallback** `private` · **yaleed-install** `private` — One-command AI workstation provisioning, free-tier model fallback chains, and full environment restore.

### Portfolio & presence
- **[Portfolio](https://yaleedhaque.github.io)** — Project index, plus WebGL portfolios: [night-temple](https://yaleedhaque.github.io/portfolio/) · [local-network](https://yaleedhaque.github.io/portfolio-hw/).
- **[Downloads hub](https://yaleedhaque.github.io/downloads/)** — Every public build in one place: apps, installers and standalone files. Source stays private.

---

## How I work

- **Offline-first by default.** Local-first isn't a slogan here — it's an architectural constraint I've applied to 30 projects. If it needs the cloud to work, it isn't finished.
- **Tests and CI as the definition of done**, not an afterthought.
- **Licensed work.** MIT or Apache-2.0 — usable in your codebase on day one.
- **Full-stack range.** Native desktop, Android, and TypeScript web, plus the networking and systems work underneath.

---

## Currently

Building on Family Tapestry (launch + export formats), sharpening the Bluetooth HID stack, improving Lumen's Morse accuracy, and lowering GamePad latency. Looking for a full-time role in C#/.NET, Android/Kotlin, or agent tooling.

---

## Contribution activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/yaleedhaque/yaleedhaque/output/github-snake-dark.svg?raw=true" />
  <img alt="Contribution graph rendered as an animated snake" src="https://raw.githubusercontent.com/yaleedhaque/yaleedhaque/output/github-snake.svg?raw=true" />
</picture>

## <a id="contact"></a>Contact

- **Portfolio:** https://yaleedhaque.github.io
- **GitHub:** https://github.com/yaleedhaque
- **Email:** `yaleedhaque` at `gmail.com` — written plainly so it isn't scraped; feel free to send it directly

I'm happy to do a technical deep-dive on any project, walk through the architecture, or run a coding conversation — whichever is useful for the role.

---

<p align="center">
  <img src="https://grs-lac.vercel.app/api?username=yaleedhaque&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" height="150">
  <img src="https://grs-lac.vercel.app/api/top-langs/?username=yaleedhaque&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" height="150">
</p>

<!--DATE-->_Md. Yaleed Haque · Dhaka, Bangladesh · Updated 2026-10-13_<!--/DATE-->
