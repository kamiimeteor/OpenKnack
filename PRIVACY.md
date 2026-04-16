# Privacy Policy

Last updated: March 10, 2026

OpenKnack is a local-first desktop application.

## What the app stores locally

- Local bridge configuration files
- Local receipt and diagnostic records created during setup flows
- Local secret files such as the Telegram bot token when you complete bridge setup

These files are stored on your device so the app can complete installation, verification, and bridge operations.

## What the app sends over the network

In the current public preview (`v0.1.1`), the app may contact:

- Telegram API endpoints to validate your bot token and send the first confirmation message
- OpenClaw installation endpoints when the selected install path requires downloading OpenClaw
- GitHub release pages when you manually download the application

## What the app does not claim to do

This public distribution repo does not publish application source code.

The current release does not advertise a hosted dashboard, cloud sync service, or centralized telemetry service for user conversations.

## Your responsibilities

- Keep your Telegram bot token private
- Review local receipt files before sharing them, because they may contain environment and setup details
- Use the official release page when downloading updates

## Contact

For privacy questions or requests, open an issue in this repository:

https://github.com/kamiimeteor/OpenKnack/issues
