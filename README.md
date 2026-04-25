<h1 align="center">🔥 TOKNORA</h1>
<p align="center"><strong>AI Spend Analytics — Desktop App + Browser Extension</strong></p>
<p align="center">
  Track token costs across Claude Code, ChatGPT, Gemini and more. Locally. Privately. No cloud.
</p>
<p align="center">
  <a href="https://github.com/ObiriecLabs/toknora/releases/latest"><img src="https://img.shields.io/github/v/release/ObiriecLabs/toknora?label=latest&color=orange" alt="Latest Release"></a>
  <img src="https://img.shields.io/badge/platform-macOS%20%7C%20Windows-blue" alt="Platform">
  <img src="https://img.shields.io/badge/price-%2439%20one--time-brightgreen" alt="Price">
  <img src="https://img.shields.io/badge/extension-free-purple" alt="Extension Free">
</p>

---

## Download

👉 **[Latest Release — v2.2.3](https://github.com/ObiriecLabs/toknora/releases/latest)**

| Platform | File | Notes |
|---|---|---|
| **macOS** | `TOKNORA-{version}-mac.dmg` | Drag to Applications |
| **macOS** (auto-installer) | `TOKNORA-installer-mac.zip` | Downloads & installs latest automatically |
| **Windows** | `TOKNORA-{version}-win-setup.exe` | Standard installer |

**Purchase:** [obirieclabs.com/toknora](https://obirieclabs.com/toknora) · $39 Mac · $49 Mac + Windows  
**Web Extension:** free — Chrome, Firefox, Edge (in review)

---

## What is TOKNORA?

TOKNORA is a local AI spend analytics app for developers. It tracks token costs and usage across **Claude Code, Claude Desktop, ChatGPT Desktop, Gemini Desktop** and more — all from a single dashboard, with no data leaving your machine.

Two products in one:

| Product | What it does |
|---|---|
| **Desktop App** | Deep analytics on Claude Code sessions + multi-AI desktop monitoring |
| **Web Extension** (free) | Token cost tracking on Claude.ai, ChatGPT, Gemini, Grok, Mistral in-browser |

**Runs completely offline.** Your data never leaves your machine.

---

## Desktop App Features

### 📊 Dashboard
The main analytics view. Shows 9 panels covering cost, tokens, sessions, cache efficiency, and activity over time.

- **Period selector:** Today · 7 days · 30 days · Month · All time
- **Filter by project** — focus on a single Claude Code project
- **Filter by AI provider** — Claude, ChatGPT Desktop, Gemini Desktop, Copilot
- **Export CSV** — download all visible data in one file

### 🔴 Live
Real-time monitoring of your current AI session. Polls every 10 seconds and shows token count, cost, and activity status (active / idle).

### ⚡ Optimize
Health score (A–F) based on 10 automated detectors. Flags issues like cache bloat, excessively long sessions, high tool call overhead, and context saturation. Each finding comes with an actionable fix button.

### 💰 Budget
Tracks your context window usage and maps it against Claude plans (Free / Pro / Max ×5 / Max ×20 / API) in real time.

### 🔀 Compare
Side-by-side comparison of two time periods. Shows delta KPIs and charts so you can measure whether your AI usage is improving over time.

---

## Desktop App Monitoring

| App | Token data |
|---|---|
| **Claude Code** | ✅ Full — reads JSONL session files |
| **Claude Desktop** | ✅ Real tokens — reads `buddy-tokens.json` |
| **ChatGPT Desktop** | ⚠️ Activity only (token count requires local proxy) |
| **Gemini Desktop** | ⚠️ Activity only (file mtime detection) |
| **Microsoft Copilot** | ⚠️ Activity only |

---

## Export Options

| Format | Description |
|---|---|
| **CSV** | All analytics tables in a single file — opens in Excel / Numbers |
| **PDF Report** | Formatted multi-page report with all sections |
| **PowerPoint** | Presentation slides with charts |
| **Audio (TTS)** | Spoken summary using your macOS system voice — no API, no internet |
| **NotebookLM Audio** | AI-generated podcast via Google NotebookLM |
| **NotebookLM Briefing** | AI-written summary document |

---

## Alerts & Notifications

| Channel | How it works |
|---|---|
| **Desktop popup** | Native macOS / Windows system notification |
| **Sound** | System beep or custom audio file (.mp3, .wav, .aiff) |
| **Email** | SMTP — works with Gmail App Passwords and most SMTP providers |
| **Telegram** | Free Telegram bot — requires a bot token + your chat ID |

### Gmail setup
1. Enable 2-factor authentication → [myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords) → create App Password for "Mail"
2. Paste the 16-character password into TOKNORA Settings → Alerts → Email

### Telegram setup
1. Open Telegram → search **@BotFather** → `/newbot` → copy bot token
2. Paste token in TOKNORA Settings → Alerts → Telegram
3. Send any message to your bot, then click the getUpdates link in Settings to find your Chat ID

---

## Settings & Keyboard Shortcuts

Press `,` to open Settings — Alerts / Export (TTS voice picker) / General tabs.

| Key | Action | Key | Action |
|---|---|---|---|
| `1–5` | Switch view | `R` | Refresh |
| `E` | Export panel | `,` | Settings |
| `?` | Help | `Esc` | Close modal |

---

## Requirements

| | Minimum |
|---|---|
| **macOS** | macOS 11 (Big Sur) or later |
| **Windows** | Windows 10 / 11 (64-bit) |
| **Disk space** | ~150 MB |
| **Internet** | Not required after activation |

---

## License

Offline HMAC-SHA256 license validation — no activation server required. Your key works permanently on the machine you activate it on.

**Lost your key?** Contact [support@obirieclabs.com](mailto:support@obirieclabs.com)

---

## Version History

| Version | Date | Highlights |
|---|---|---|
| **v2.2.3** | 2026-04-25 | Voice picker TTS, email fix, clickable links in settings, language selector fix |
| v2.2.2 | 2026-04-24 | Optimize actions, MCP remove confirmation |
| v2.2.1 | 2026-04-24 | AI provider filter, desktop app monitoring |
| v2.2.0 | 2026-04-24 | TOKNORA Web Extension (Chrome, Firefox, Edge) |
| v2.1.9 | 2026-04-24 | Parser improvements, token deduplication |

[Full changelog →](https://github.com/ObiriecLabs/toknora/releases)

---

<p align="center">
  <strong>Obiriec Labs © 2026</strong> · <a href="https://obirieclabs.com/toknora">obirieclabs.com/toknora</a> · <a href="mailto:support@obirieclabs.com">support@obirieclabs.com</a>
</p>
