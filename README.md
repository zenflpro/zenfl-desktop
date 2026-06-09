# Zenfl — Desktop Auto-Apply Agent

The Zenfl desktop app applies to Upwork jobs for you. When you tap **⚡ Auto Apply** on a job (in the Zenfl Telegram bot or dashboard), this app opens the job in **your own Google Chrome**, writes an AI-generated proposal from your profile, and submits it — respecting your bid strategy and guardrails.

This repository hosts the **official installers and the auto-update feed**. The app's source code lives in Zenfl's main repository.

## Download

Get the latest installer for your OS from the **[latest release](https://github.com/zenflpro/zenfl-desktop/releases/latest)**:

- **macOS** — `.dmg`
- **Windows** — `Setup .exe`
- **Linux** — `.AppImage`

## Requirements

- A **Zenfl account** — sign up at https://app.zenfl.pro
- An **Upwork account** you can log into
- **Google Chrome** installed (the app automates your real Chrome)
- macOS 11+, Windows 10/11, or a modern Linux distro

## Install

The app isn't code-signed yet (beta), so your OS will show a warning the first time. This is expected.

### macOS

1. Open the `.dmg` and drag **Zenfl** to **Applications**.
2. On first launch macOS may say **"Zenfl.app is damaged and can't be opened."** It isn't damaged — macOS just blocks unsigned apps downloaded from the internet. Clear it once with these steps:
   1. Open **Terminal**: press **⌘ (Command) + Space**, type **Terminal**, and press **Enter**.
   2. In Terminal, type the following exactly — **including the space at the end** — but **don't press Enter yet**:
      ```
      xattr -dr com.apple.quarantine 
      ```
   3. Open your **Applications** folder, then **drag the Zenfl app into the Terminal window**. Its location fills in automatically. Now press **Enter**.
   4. Open **Zenfl** from Applications as usual. You only need to do this once.

### Windows

1. Run the `Setup .exe`.
2. If Windows SmartScreen appears, click **More info → Run anyway**.

### Linux

1. Make the AppImage executable: `chmod +x ./Zenfl-*.AppImage`
2. Run it: `./Zenfl-*.AppImage`

## Getting started

1. **Install Google Chrome** (if you haven't) and the desktop app above.
2. In the Zenfl dashboard, open **[Auto Apply](https://app.zenfl.pro/auto-apply)** → **Connect device**, then enter the pairing code in the app.
3. **Import and complete your Upwork profile** on the [Profile page](https://app.zenfl.pro/profile). Proposals are generated from this — the richer your experience and skills, the better they read.
4. **Open the browser** in the desktop app and sign in to Upwork once. Your session stays on your machine.
5. Set your **bid strategy and guardrails** in [Auto-apply settings](https://app.zenfl.pro/auto-apply/settings).
6. Tap **⚡ Auto Apply** on a matching job in Telegram — your active device applies in the background.

## How it works & why it's safe

- **Your credentials never leave your machine.** The app uses your already-logged-in Upwork session in your own browser. Zenfl never sees or stores your Upwork password.
- **Undetectable by Upwork.** It drives a normal Google Chrome — not a browser extension or injected script. There's nothing to detect: it's the same browser you'd use yourself, just automated.
- **It applies like you would.** Human-like typing and clicks, and it never bids below your rate floor, over your Connects cap, or past your daily limit.
- **You stay in control.** One active device at a time, disconnect anytime, and every attempt shows up in your history.

## Updates

- **Windows & Linux** update automatically in the background and install on quit.
- **macOS** auto-update is disabled until the app is code-signed — until then, re-download the latest `.dmg` from the [releases page](https://github.com/zenflpro/zenfl-desktop/releases/latest).

## Pricing

50 credits per submitted application — a reduced beta price (80 credits normally). You're charged when the proposal is sent and automatically refunded if the agent couldn't submit (job closed, not logged in, needs review, etc.).

## Support

Questions or issues? Visit **https://app.zenfl.pro/support**.

---

© Zenfl. All rights reserved.
