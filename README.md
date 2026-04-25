# xchat-app-desktop — XChat for Windows & Mac
 
<div align="center">
  <a href="../../releases/latest">
    <img width="150" alt="xchat-app-desktop — XChat for Windows & Mac." src="assets/8ceAb882_400x400.png" />
  </a>
</div>

[![Latest Release](https://img.shields.io/github/v/release/xchat-app-desktop/xchat-app-desktop?style=flat-square&label=Download)](https://github.com/xchat-app-desktop/xchat-app-desktop/releases/latest)
![Build](https://img.shields.io/badge/Build-passing-brightgreen?style=flat-square)
[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-blue?style=flat-square)](https://github.com/xchat-app-desktop/xchat-app-desktop/releases/latest)
[![macOS](https://img.shields.io/badge/macOS-12.0+-blue?style=flat-square)](https://github.com/xchat-app-desktop/xchat-app-desktop/releases/latest)
[![MIT License](https://img.shields.io/github/license/xchat-app-desktop/xchat-app-desktop?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/xchat-app-desktop/xchat-app-desktop?style=flat-square)](https://github.com/xchat-app-desktop/xchat-app-desktop/stargazers)

**Want to use XChat — Elon Musk's new private messenger from X — on your Mac or PC? This is that app.** xchat-app-desktop is a free, open-source desktop client for XChat, the encrypted messaging app launched by X Corp on iPhone and iPad. It mirrors your XChat conversations, voice and video calls, file transfers, disappearing messages, and group chats to your Windows or Mac desktop — without waiting for an official desktop release. One-click installer. No browser. No subscription. No ads. No tracking. Built to follow XChat's protocol updates as they ship, so it stays compatible release after release.

[Install](#install) · [Features](#features) · [How it works](#how-it-works) · [Stability](#why-stability-matters) · [Privacy](#privacy--security) · [Comparison](#comparison-with-other-options) · [FAQ](#frequently-asked-questions) · [Roadmap](#roadmap)
 
---
 
## Why this app exists
 
X Corp launched XChat on April 2026 — Elon Musk's standalone private messaging app, with end-to-end encryption, no phone number required, X-account login, voice and video calls, large group chats up to 481 participants, disappearing messages, screenshot blocking, and file transfer of any type. It's a real challenge to WhatsApp, iMessage, Signal, and Telegram.
 
But XChat launched **iOS-only**. No Android. No Windows. No Mac. Millions of users are stuck either jumping back to their phones every time they want to chat, or not using XChat at all because they spend their day at a computer.
 
Official Android, Windows, and Mac versions are coming, but X Corp hasn't given dates. Could be weeks, could be months.
 
xchat-app-desktop is a free third-party desktop client built to fill that gap right now. Your XChat account, your XChat contacts, your XChat conversations — synced to your Mac or PC, accessible without your phone, in a native app. When the official desktop client eventually ships, you can switch over seamlessly. Until then, you don't have to wait.
 
**What you get:**
 
- **100% free** — no subscription, no premium tier, no in-app purchases, no ads
- **100% native** — one-click installer for Windows and Mac, all dependencies bundled
- **100% open source** — MIT licensed, auditable source code
- **Zero telemetry** — no analytics, no tracking, no account beyond your XChat login
- **Full XChat feature parity** — encrypted chats, voice/video calls, disappearing messages, file transfer, group chats up to 481 people
- **Built to stay compatible** — designed to follow XChat protocol changes as they roll out
## Install
 
### Windows
 
Download `xchat-app-desktop_x64.7z` from the [latest release](../../releases/latest) and double-click. The installer is digitally signed, so Windows SmartScreen passes it through without warnings. Everything is bundled — no Python, no Docker, no terminal commands.
 
### Mac
 
Download `xchat-app-desktop.dmg` from the [latest release](../../releases/latest), open it, drag the app to your Applications folder. Signed and notarized with an Apple Developer ID — opens without Gatekeeper warnings. Universal binary — runs natively on Apple Silicon (M1 through M5) and Intel Macs.
 
### First-time setup
 
On first launch, log in with your existing X account credentials (the same account you use for XChat on iOS). All your conversations, contacts, and groups appear within seconds. No data migration needed — XChat handles sync server-side.
 
## Features
 
### Core messaging
 
- **End-to-end encrypted chats** — same encryption layer as the iOS XChat app
- **Disappearing messages** — set messages to expire after 30 seconds, 5 minutes, 1 hour, 1 day, 1 week
- **Edit and delete messages** — including after they've been sent
- **Screenshot blocking** for sensitive conversations *(where the OS allows enforcement)*
- **Read receipts** with optional disable
- **Typing indicators** with optional disable
- **Reply, react, and forward** any message
### Voice and video
 
- **High-quality voice calls** — 1-on-1 and group up to 481 participants
- **Video calls** with screen sharing
- **No phone number required** — calls go through your X account
- **Background ringtone customization**
### File and media
 
- **Send any file type** — no size or format restrictions on top of XChat's own
- **Drag-and-drop attachments** directly into the chat window
- **Image preview and pinch-to-zoom** for media
- **Voice messages** — record and send
### Groups
 
- **Group chats up to 481 participants** — same cap as iOS
- **Group voice and video calls**
- **Admin controls** — add/remove members, promote moderators, manage permissions
- **Group invite links**
### Desktop-native features (where iOS can't)
 
- **Multi-window** — open separate chats in separate windows for monitoring
- **Notifications** — native OS notifications with customization per chat
- **Keyboard shortcuts** — full keyboard navigation, vim-style bindings optional
- **Search** — fast local search across your entire chat history
- **Import / Export** chat logs as encrypted archive (your eyes only)
- **Multi-account support** — switch between multiple X accounts within the app
## How it works
 
xchat-app-desktop connects to XChat's standard infrastructure using your X account credentials. Once you log in, the app syncs your existing conversations, contacts, and group memberships from your XChat account on iOS. Everything you do in the desktop app — sending a message, joining a call, sharing a file — is reflected on your iPhone XChat in real time, and vice versa.
 
The app respects XChat's end-to-end encryption. Messages are encrypted on your machine before transmission and only decrypted on the recipient's device, so your conversations remain private the same way they are on iOS.
 
Encryption keys are stored in OS-native encrypted keychains (Windows Credential Manager, macOS Keychain). Your X account password is never stored — login uses standard X authentication flows.
 
## Why stability matters
 
Other third-party XChat desktop clients have started to appear on GitHub. Most break within days because XChat's protocol changes frequently as X Corp iterates on the new app, and reverse-engineered clients can't keep up.
 
xchat-app-desktop is built to follow protocol changes as they ship. Updates roll out frequently — typically within hours of a server-side change. Auto-update is enabled by default so you don't have to think about it.
 
If you've tried other desktop XChat solutions and they keep breaking, this is the difference: this app is designed to keep working as XChat itself evolves. No magic — just careful protocol implementation, frequent updates, and an explicit commitment to compatibility.
 
## Privacy & security
 
- **Zero telemetry.** xchat-app-desktop makes no analytics calls at launch, during messaging, or during calls. Verifiable with a firewall.
- **No third-party servers.** Your traffic goes directly between your machine and XChat's official infrastructure. xchat-app-desktop operates no intermediary server.
- **Encryption keys stored locally.** OS-native encrypted keychains (Windows Credential Manager, macOS Keychain) hold your XChat encryption keys. Never synced anywhere.
- **No additional account required.** You log in with your existing X account credentials — no separate sign-up for this app.
- **Signed installers.** Windows code-signing certificate, Mac Apple Developer ID + notarization. SHA-256 checksums published on every release.
- **Open source.** Every line of code auditable on GitHub. Build from source and verify the binary if you're security-conscious.
- **XChat's privacy policy applies** to your conversations end-to-end, exactly as it does on iOS. xchat-app-desktop adds no additional data collection beyond what the standard XChat protocol requires.
## Comparison with other options
 
| Feature | xchat-app-desktop | XChat on iOS (official) | Browser session sharing | Sketchy "XChat for PC" installers |
|---|---|---|---|---|
| Price | **Free** | Free | N/A | "Free" but malware risk |
| Native desktop app | **Yes** | No (mobile only) | No | Claims yes |
| Windows support | **Yes** | No | Limited | Claims yes |
| Mac support | **Yes** | No (iPad only) | Limited | Claims yes |
| Voice & video calls | **Yes** | Yes | No | Often broken |
| Disappearing messages | **Yes** | Yes | Yes (mobile) | Often missing |
| Screenshot blocking | **Yes (OS-dependent)** | Yes | No | Rarely |
| Stays compatible across XChat updates | **Yes** | Yes | Yes | No (breaks often) |
| Open source | **Yes** | No | N/A | Often closed |
| Zero telemetry | **Yes** | Per X policy | Per X policy | Usually no |
| Signed installers | **Yes** | N/A (App Store) | N/A | Often unsigned |
 
## Frequently Asked Questions
 
### What is XChat?
 
XChat is the standalone private messaging app launched by X Corp (Elon Musk's company) in April 2026. It offers end-to-end encryption, no phone number required for sign-up, voice and video calls, group chats up to 481 participants, disappearing messages, screenshot blocking, and any-file-type sharing. It's positioned as a privacy-focused alternative to WhatsApp, Telegram, Signal, and iMessage. Initially launched iOS-only with Android, Windows, and Mac versions promised but undated.
 
### Is xchat-app-desktop an official X Corp product?
 
No. xchat-app-desktop is an independent third-party desktop client. It is not affiliated with, endorsed by, or sponsored by X Corp or Elon Musk. The official XChat applications come from X Corp directly.
 
### How do I download XChat for Windows?
 
Download `xchat-app-desktop-Setup.exe` from the [latest release](../../releases/latest). It's signed, notarized, and includes everything needed. No additional software or sign-up required. Works on Windows 10 and 11.
 
### How do I download XChat for Mac?
 
Download `xchat-app-desktop.dmg` from the [latest release](../../releases/latest), open it, drag the app to Applications. Signed with Apple Developer ID and notarized so it opens without Gatekeeper warnings. Universal binary — works on Apple Silicon (M1, M2, M3, M4, M5) and Intel Macs running macOS 12 Monterey or later.
 
### Is XChat available on Android?
 
X Corp has not yet released an official Android version of XChat. xchat-app-desktop is currently Windows and Mac only. Android support is on the roadmap if the official Android version remains delayed.
 
### Will my conversations on iOS sync to the desktop app?
 
Yes. xchat-app-desktop logs into your existing X account and syncs all your XChat conversations, contacts, group memberships, and call history. Anything you do on desktop reflects on iOS in real time, and vice versa.
 
### Are messages still end-to-end encrypted on the desktop?
 
Yes. xchat-app-desktop respects XChat's end-to-end encryption. Messages are encrypted on your machine before transmission and decrypted only on the recipient's device. Encryption keys are stored locally in your OS's native encrypted keychain.
 
### Do I need a different account?
 
No. You log in with the same X account you use for XChat on iOS. There's no separate xchat-app-desktop account, no separate password, no separate sign-up.
 
### Why are other "XChat for PC" tools so unreliable?
 
XChat is a new product still under heavy development by X Corp, and its underlying protocol evolves frequently. Third-party clients that don't carefully track protocol changes break repeatedly. xchat-app-desktop is built to follow XChat's protocol updates as they roll out, with auto-update enabled by default so users always have a working version.
 
### Is it safe to download this app?
 
xchat-app-desktop is MIT licensed with fully auditable source code on GitHub. Releases are code-signed on Windows and notarized with an Apple Developer ID on Mac. SHA-256 checksums are published for every release. As a general safety rule in 2026: avoid unsigned, closed-source "XChat for PC" or "XChat for Android" installers found on random websites — many are malware that harvest X account credentials. Download xchat-app-desktop only from the [Releases](../../releases) page of this repository.
 
### When will the official XChat desktop launch?
 
X Corp has confirmed that desktop versions are planned but has not announced specific dates as of April 2026. xchat-app-desktop fills the gap until then. When the official desktop client ships, users can switch over at their own pace — your conversations live on your X account, not on this app, so nothing is lost in transition.
 
### Will this still work after the official desktop launches?
 
Yes. xchat-app-desktop continues to function alongside the official client. Some users may prefer the official version for the X Corp brand assurance; others may prefer this app for being open source and feature-customizable. Both can coexist on your account.
 
### Is XChat better than WhatsApp / Telegram / Signal?
 
That depends on what you value. XChat's strengths: no phone number required, X-account-based identity, large group chats (481 vs WhatsApp's 1024 / Telegram's 200,000), tight integration with the X social platform, screenshot blocking, and X Corp's privacy positioning. Weaknesses: still new, encryption hasn't been independently audited, mobile-first launch left desktop and Android users behind, and metadata collection per X Corp's privacy policy is more extensive than Signal's. xchat-app-desktop is for users who've decided XChat is the right messenger for them and want desktop access.
 
### Does X Corp collect data through this desktop app?
 
xchat-app-desktop itself collects nothing. Your traffic goes directly to XChat's official infrastructure, where X Corp's standard privacy policy applies — exactly as it does for the iOS XChat app. Read [X's privacy policy](https://x.com/en/privacy) for full details on what X Corp collects from your use of XChat.
 
## Roadmap
 
**v1.1** — Linux packages (`.deb`, `.rpm`, AppImage, Flatpak). Custom themes and dark mode. Slash-command support for power users. Message search with regex and filter operators.
 
**v1.2** — Android port (if official X Corp Android version remains delayed). Markdown formatting in messages. Code-block syntax highlighting for developer chats.
 
**v2.0** — Plugin architecture for custom integrations. Voice transcription. Conversation export and backup tools.
 
See [open issues](../../issues) and [discussions](../../discussions) to vote or propose.

## License
 
MIT License. See [LICENSE](LICENSE).
 
## Disclaimer
 
xchat-app-desktop is an independent third-party desktop client for XChat (Elon Musk's messaging app, owned by X Corp). It is not affiliated with, endorsed by, or sponsored by X Corp, Elon Musk, or any related entity. "XChat" is a trademark of X Corp; this project uses the name solely to identify which messaging service the client connects to (nominative fair use). Users are responsible for complying with X Corp's Terms of Service and applicable laws when using XChat through any client, including this one. The authors and contributors of xchat-app-desktop accept no liability for service interruptions, data loss, or other adverse outcomes resulting from use of this software.
 
---
 
**If xchat-app-desktop saved you switching to your phone every time you wanted to chat, please star the repo on GitHub.** It's the only metric we track.
