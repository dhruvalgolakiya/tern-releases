# Tern

Downloads and the update feed for Tern, a fast native Gmail client for macOS. Mail lives in a local database, so
opening, searching and labelling never wait on the network; several Gmail and Google Workspace accounts share one
inbox.

## Download

Get the latest `Tern-<version>.dmg` from [Releases](https://github.com/dhruvalgolakiya/tern-releases/releases/latest),
open it and drag Tern to Applications. Tern is signed with a Developer ID and notarized by Apple.

- An Apple Silicon Mac on macOS 15 or later.
- Your own Google Cloud OAuth client of type "Desktop app" with the Gmail API turned on. Tern ships without one;
  [SETUP.md](SETUP.md) walks through it in about ten minutes. Tern keeps it in your Mac's Keychain.
- Optional, for AI: the Claude Code (`claude`) or Codex (`codex`) command-line tool, signed in with your own plan.

## Updates

Tern updates itself from this repository: it reads `appcast.xml` from the latest release, downloads the new version
in the background and installs it when you restart or quit. Each update is signed, and Tern refuses one whose
signature doesn't match.
