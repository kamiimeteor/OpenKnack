# AI Gene Capsule

<p align="center">
  <img src="assets/gene_capsule_logo.png" alt="AI Gene Capsule" width="320" />
</p>

<p align="center">
  <a href="https://github.com/kamiimeteor/AI-Gene-Capsule/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/kamiimeteor/AI-Gene-Capsule?display_name=tag"></a>
  <a href="https://github.com/kamiimeteor/AI-Gene-Capsule/releases"><img alt="Total downloads" src="https://img.shields.io/github/downloads/kamiimeteor/AI-Gene-Capsule/total"></a>
  <img alt="Platform" src="https://img.shields.io/badge/platform-macOS%20arm64-111827">
  <img alt="License" src="https://img.shields.io/badge/license-Proprietary-b91c1c">
</p>

**The local host for installable AI workflows.**

AI Gene Capsule turns complex local automations into installable capsules with setup, permissions, receipts, and ongoing runtime. It is not another chat assistant — it is the host layer that makes AI integrations deployable local software.

## Quick Links

- [Download latest release](https://github.com/kamiimeteor/AI-Gene-Capsule/releases/latest)
- [Changelog](CHANGELOG.md)
- [Security policy](SECURITY.md)
- [Privacy policy](PRIVACY.md)
- [Contributing](CONTRIBUTING.md)
- [Code of conduct](CODE_OF_CONDUCT.md)

## Download

| Platform | Architecture | Download |
|----------|-------------|----------|
| macOS | Apple Silicon (arm64) | [AI Gene Capsule v0.1.1](https://github.com/kamiimeteor/AI-Gene-Capsule/releases/latest) |

> More platforms (Intel macOS, Windows, Linux) coming soon.

### Install on macOS

1. Download the `.dmg` file from the [Releases](https://github.com/kamiimeteor/AI-Gene-Capsule/releases) page
2. Open the `.dmg` and drag **AI Gene Capsule** to your Applications folder
3. Launch the app — if macOS blocks it, go to **System Settings > Privacy & Security** and click **Open Anyway**

## System Requirements

- macOS 14+ recommended
- macOS on Apple Silicon (`arm64`)
- Current public preview supports the **OpenClaw + Telegram** setup path only
- A Telegram bot token from **@BotFather** is required for bridge setup
- Before running Telegram setup, open your bot in Telegram and tap **Start** once
- Internet access is required during setup for Telegram API validation and, in some install paths, OpenClaw installation

## Verify Download

For `AI Gene Capsule-0.1.1-arm64.dmg`:

```text
134a3bfe263532f588a4fabe4a7cdac9a0a25032c238f171e6104a3afa3a9d99
```

On macOS:

```bash
shasum -a 256 "AI Gene Capsule-0.1.1-arm64.dmg"
```

The output should match the checksum published in [SHA256SUMS.txt](SHA256SUMS.txt).

## What It Does

AI Gene Capsule v0.1.1 provides the first end-to-end public workflow:

1. **Environment Check** — Diagnose whether your machine is ready for OpenClaw
2. **OpenClaw Install** — Install or verify OpenClaw locally
3. **Telegram Bridge** — Connect Telegram with a guided bridge flow
4. **Receipts** — Review local receipts and diagnostics for every action

## Screenshots

### OpenClaw Landing

![OpenClaw landing](assets/screenshots/01-openclaw-home.png)

### Telegram Bridge Setup

![Telegram bridge setup](assets/screenshots/02-telegram-setup.png)

### Setup Complete

![Setup complete](assets/screenshots/03-setup-complete.png)

## What AI Gene Capsule Is

AI Gene Capsule is a desktop host for installable AI workflows. Instead of giving users a blank agent, it gives them **capsules** that set up and run a specific local integration — like OpenClaw + Telegram — with explicit permissions, diagnostics, and ongoing status.

The product should feel like:
- **Install** → **Connect** → **Run** → **Monitor** → **Repair**

Not like: open chat → type anything → hope the agent figures it out.

## Product Flow

![AI Gene Capsule product flow](assets/diagrams/concept-flow.svg)

This public repo intentionally shows the product flow, not the internal implementation. The current desktop path is:

1. Install the desktop app
2. Check whether the machine is ready
3. Install or verify OpenClaw
4. Connect Telegram
5. Run locally
6. Review receipts and recover when needed

## Current Scope (v0.1.1)

**Included:**
- Quick Start flow in the desktop console
- Manual Mode for readiness, install, and Telegram bridge
- Telegram bridge token validation and first-message confirmation
- Receipt generation for install and bridge actions

**Not yet included:**
- Discord bridge
- Lark / Feishu bridge
- Notarized macOS distribution
- Intel macOS, Windows, and Linux builds

## Troubleshooting

- **macOS says the app cannot be opened**
  Go to **System Settings > Privacy & Security** and click **Open Anyway**. `v0.1.1` is a pre-release and is not notarized yet.
- **Telegram connect does not send the first message**
  Open your bot in Telegram, tap **Start**, then rerun **Connect Telegram**.
- **The bot token is rejected**
  Make sure you pasted the full BotFather token, including the numeric prefix and the colon.
- **This Mac is Intel, not Apple Silicon**
  The current public build is `arm64` only. Intel macOS support is not published yet.

## Roadmap

- [ ] Discord bridge capsule
- [ ] Lark / Feishu bridge capsule
- [ ] Notarized macOS distribution
- [ ] Windows and Linux desktop packages
- [ ] Managed registry and hosted updates

## What May Become Paid Later

The desktop app and local capsule runtime are **free**.

Future paid offerings are expected to sit above the local host:
- Managed registry or hosted updates
- Managed bridge hosting
- Team features and shared operations
- Cloud monitoring and audit trails
- Commercial support and enterprise controls

## Community & Support

- [Issues](https://github.com/kamiimeteor/AI-Gene-Capsule/issues) for bugs, install problems, and feature requests
- [Releases](https://github.com/kamiimeteor/AI-Gene-Capsule/releases) for new desktop builds
- [Security policy](SECURITY.md) for responsible vulnerability reporting

## Feedback & Issues

Found a bug or have a feature request? Please [open an issue](https://github.com/kamiimeteor/AI-Gene-Capsule/issues).

For privacy details, see [PRIVACY.md](PRIVACY.md).

## License

This software is proprietary. See [LICENSE](LICENSE) for details.

Free to download and use. Source code is not included or available in this repository.
