<p align="center">
  <img src="https://obirieclabs.com/static/img/toknora-icon.png" width="80" alt="TOKNORA logo">
</p>

<h1 align="center">TOKNORA</h1>
<p align="center"><strong>Claude Code Analytics — Desktop App</strong></p>
<p align="center">
  Track costs, sessions, and performance of your Claude Code usage. Locally. Privately. No cloud.
</p>
<p align="center">
  <a href="https://github.com/ObiriecLabs/toknora-releases/releases/latest"><img src="https://img.shields.io/github/v/release/ObiriecLabs/toknora-releases?label=latest&color=orange" alt="Latest Release"></a>
  <img src="https://img.shields.io/badge/platform-macOS%20%7C%20Windows-blue" alt="Platform">
  <img src="https://img.shields.io/badge/price-%2439%20one--time-brightgreen" alt="Price">
</p>

---

## Download

👉 **[Latest Release — v2.2.3](https://github.com/ObiriecLabs/toknora-releases/releases/latest)**

| Platform | File | Notes |
|---|---|---|
| **macOS** | `TOKNORA-{version}-mac.dmg` | Drag to Applications |
| **macOS** (auto-installer) | `TOKNORA-installer-mac.zip` | Downloads & installs latest automatically |
| **Windows** | `TOKNORA-{version}-win-setup.exe` | Standard installer |

**Purchase:** [obirieclabs.com/toknora](https://obirieclabs.com/toknora) · $39 Mac · $49 Mac + Windows

---

## What is TOKNORA?

TOKNORA is a desktop analytics app that reads your Claude Code session files from `~/.claude/projects/` and turns them into rich, interactive dashboards — without sending any data to external servers.

Think of it as the GUI version of `npx codeburn`, but with 5 views, real-time monitoring, export options, and smart optimization tips.

**Runs completely offline.** Your data never leaves your machine.

---

## Features

### 📊 Dashboard
The main analytics view. Shows 9 panels covering cost, tokens, sessions, cache efficiency, and activity over time.

- **Period selector:** Today · 7 days · 30 days · Month · All time
- **Filter by project** — focus on a single Claude Code project
- **Filter by AI provider** — Claude, ChatGPT Desktop, Gemini Desktop, Copilot
- **Export CSV** — download all visible data in one file

### 🔴 Live
Real-time monitoring of your current Claude Code session. Polls every 10 seconds and shows token count, cost, and activity status (active / idle).

### ⚡ Optimize
Health score (A–F) based on 10 automated detectors. Flags issues like:
- Cache bloat (cache writes >> cache reads)
- Excessively long sessions
- High tool call overhead
- Context saturation
- Repeated patterns

Each finding comes with an actionable fix button.

### 💰 Budget
Tracks your context window usage and maps it against Claude plans:
- Free / Pro / Max ×5 / Max ×20 / API
- Shows current usage vs plan limits in real time

### 🔀 Compare
Side-by-side comparison of two time periods. Shows delta KPIs and charts so you can see if your Claude usage is improving over time.

---

## Export Options

Access from the **Export** button (top right) or press `E`.

| Format | Description |
|---|---|
| **CSV** | All analytics tables in a single file — opens in Excel / Numbers |
| **PDF Report** | Formatted multi-page report with all sections |
| **PowerPoint** | Presentation slides with charts |
| **Audio (TTS)** | Spoken summary using your macOS system voice — no API, no internet |
| **NotebookLM Audio** | AI-generated podcast via Google NotebookLM *(requires `notebooklm login`)* |
| **NotebookLM Briefing** | AI-written summary document |

For **Audio (TTS)**, you can choose any macOS system voice from the voice picker in Settings → Export.

---

## Alerts & Notifications

Configure in **Settings → Alerts** (press `,`).

| Channel | How it works |
|---|---|
| **Desktop popup** | Native macOS / Windows system notification |
| **Sound** | System beep or custom audio file (.mp3, .wav, .aiff) |
| **Email** | SMTP — works with Gmail App Passwords and most SMTP providers |
| **Telegram** | Free Telegram bot — requires a bot token + your chat ID |

### Gmail setup
1. Enable 2-factor authentication on your Google account
2. Go to [myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords)
3. Create an App Password for "Mail"
4. Paste the 16-character password into TOKNORA Settings → Alerts → Email

### Telegram setup
1. Open Telegram and search for **@BotFather**
2. Send `/newbot` and follow the instructions to create a bot
3. Copy the bot token and paste it in TOKNORA Settings → Alerts → Telegram
4. Send any message to your new bot, then click the **getUpdates** link in Settings to find your Chat ID

---

## Settings

Press `,` to open Settings.

**Alerts tab** — configure popup, sound, email, and Telegram notifications.  
**Export tab** — set default export path and TTS voice.  
**General tab** — auto-refresh interval, theme, default start tab.

---

## Keyboard Shortcuts

| Key | Action |
|---|---|
| `1` | Dashboard |
| `2` | Live |
| `3` | Optimize |
| `4` | Budget |
| `5` | Compare |
| `R` | Refresh |
| `E` | Export panel |
| `,` | Settings |
| `?` | Help |
| `Esc` | Close modal |

---

## Requirements

| | Minimum |
|---|---|
| **macOS** | macOS 11 (Big Sur) or later |
| **Windows** | Windows 10 / 11 (64-bit) |
| **Claude Code** | Any version — reads `~/.claude/projects/*.jsonl` |
| **Disk space** | ~150 MB |
| **Internet** | Not required (pricing cache uses LiteLLM, updates checked on startup) |

---

## Desktop App Monitoring

TOKNORA can also track usage from other AI desktop apps:

| App | Token data |
|---|---|
| **Claude Code** | ✅ Full — reads JSONL session files |
| **Claude Desktop** | ✅ Real tokens — reads `buddy-tokens.json` |
| **ChatGPT Desktop** | ⚠️ Activity only (token count requires local proxy) |
| **Gemini Desktop** | ⚠️ Activity only (file mtime detection) |
| **Microsoft Copilot** | ⚠️ Activity only |

---

## License

TOKNORA uses offline HMAC-SHA256 license validation — no activation server required.  
Your license key works permanently, on the machine you activate it on.

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

[Full changelog →](https://github.com/ObiriecLabs/toknora-releases/releases)

---

## Web Extension

TOKNORA is also available as a browser extension for tracking token usage directly on Claude.ai, ChatGPT, Gemini, and other AI web apps.

**Status:** In review on Chrome Web Store, Edge Add-ons, and Firefox AMO.

---

<p align="center">
  <strong>Obiriec Labs © 2026</strong> · <a href="https://obirieclabs.com/toknora">obirieclabs.com/toknora</a> · <a href="mailto:support@obirieclabs.com">support@obirieclabs.com</a>
</p>
