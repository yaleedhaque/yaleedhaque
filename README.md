<h1 align="center">
  <a href="https://yaleedhaque.github.io">
    <img src="https://yaleedhaque.github.io/banner.png" width="100%" alt="Md. Yaleed Haque — C#/.NET and Kotlin/Android engineer, Dhaka, Bangladesh">
  </a>
  <br><br>
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

> **Note on access:** source for several projects below is private by default. Each is marked `🔒` — the code is available on request, and I can walk through the architecture live. Repositories without the marker are public and open to review right now.

### Desktop automation & AI agents
- **StarkAgent** 🔒 — Fully autonomous Windows desktop control agent. **295+ commands** across mouse, keyboard, OCR, UIA tree-walking, file operations, web fetch, and email, exposed over a local TCP/JSON API. Includes a WhatsApp driver and MCP server. *(C# · 15.5k LOC · MIT)*
- **yale-agent** 🔒 — Wayland-native Linux desktop agent: **68 tools** in 11 categories (vision click-by-text, browser, desktop, media, audio, filesystem, system) via MCP server, CLI, and web dashboard. Solved Wayland input injection and GNOME screenshot access without a display server hack. *(Python)*
- **AI Browser Toolkit** 🔒 — Let an AI agent drive real Chrome or Edge over a JSON API. One server, one persistent profile, full DOM control. **347 tests.** *(Python · Apache-2.0)*
- **precise-hands** 🔒 — MCP server for exact-coordinate automation: AT-SPI and XDG portal for Linux desktop, uiautomator bounds → `input tap` for Android. Built because screenshot-guessing clicks caused misclicks. *(Python)*
- **[NetSpeedBar](https://yaleedhaque.github.io)** — Always-on-top taskbar network overlay with single named-mutex instance handling. *(C#)*

### Android / Kotlin
- **BluetoothRemoteHid** 🔒 — Turn a phone into a wireless keyboard, touchpad, air-mouse and media remote for any PC over **Bluetooth Classic + LE HID**. No host software, no cloud. Implemented the HID report-descriptor and pairing layers directly. *(Kotlin)*
- **GamePadEcosystem** 🔒 — Android phones as wireless Xbox 360 controllers. **Sub-5 ms latency**, offline multiplayer, zero cloud. *(C# host + Kotlin)*
- **Lumen** 🔒 — Offline torch: LED, screen light, strobe, SOS, Morse send, and **Morse decode from the camera** via ML Kit. *(Kotlin + Compose)*
- **AetherCompass** 🔒 — Feature-packed offline compass with accurate bearings. *(Kotlin + Compose)*
- **OmniFetch-Android** 🔒 — Search, stream and download video on-device with a bundled yt-dlp + ffmpeg engine and a gesture player. *(Kotlin + Compose)*

### Web & product
- **Family Tapestry** 🔒 — Collaborative graph-based family tree: real-time presence, timeline, map, generations, sub-tree collapse, multi-format export. Next.js + TypeScript + Supabase (RLS) + React Flow + Leaflet. **239 tests, 27.8k LOC, 7 migrations.** **[Live →](https://family-tapestry-nine.vercel.app)**
- **bKash + WhatsApp Storefront** 🔒 — Sellable e-commerce template for Bangladeshi local shops: manual bKash payment, WhatsApp order flow, stock, categories, admin dashboard. **[Live →](https://bkash-ecommerce.vercel.app)**
- **[YaleDoc](https://github.com/yaleedhaque/yale-doc-yaleed)** — Self-encrypting documents in **one HTML file**. AES-256-GCM, PBKDF2-SHA256, encrypted version history, attachments, English/বাংলা UI, zero dependencies, opens offline anywhere. **Verified on Chromium, Firefox and WebKit.**
- **[ProctorFree](https://github.com/yaleedhaque/proctor-free)** — Browser-based exam proctoring where all AI runs client-side. No servers, no tracking.

### Systems & networking
- **[YaleVPN-PC](https://github.com/yaleedhaque/YaleVPN-PC)** — Desktop WireGuard + Cloudflare WARP client for Linux and Windows: on-device keys, egress IP rotation, kill switch, DNS pinning, GUI + CLI. *(Python)*
- **[yalevpn](https://github.com/yaleedhaque/yalevpn)** — WireGuard VPN + Shizuku integration research lab for Android. *(Kotlin)*
- **stark-hotspot** 🔒 — Run a WiFi hotspot while staying connected to WiFi: concurrent STA+AP on one radio (hostapd + dnsmasq + NAT). *(Shell)*
- **Edge** 🔒 — Self-hosted on-device speech-to-text. Word-timed transcripts with clickable words, txt/srt/vtt export, faster-whisper + ffmpeg. No cloud, no API keys. *(Python)*
- **haque-squad** 🔒 — Authoritative-server multiplayer arena shooter (Godot 4) with phone browser touch controllers over WebSocket. *(GDScript)*

### AI tooling & agent infrastructure
- **opencode-dotfiles** 🔒 — Version-controlled AI agent brain: config, scripts, skills, memory, research, systemd units. Secrets handled through an encrypted vault with one passphrase held outside the repo.
- **opencode-setup-kit** 🔒 · **opencode-free-fallback** 🔒 · **yaleed-install** 🔒 — One-command AI workstation provisioning, free-tier model fallback chains, and full environment restore.

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

<!--DATE-->_Md. Yaleed Haque · Dhaka, Bangladesh · Updated 2026-10-05_<!--/DATE-->
