<img src="logo.png" width="96" alt="BE-Mail">

# BE-Mail - releases

Download and update channel for **BE-Mail**, a simple, fast and secure mail and calendar
client for Office 365 (Tauri + Rust).

This repository holds nothing but release artifacts. It is public because the app's built-in
updater needs somewhere it can reach without a token.

## Install

Take the installer from the **[latest release](../../releases/latest)** - under **Assets**,
`BE-Mail_x.y.z_x64-setup.exe`.

| Asset | Purpose |
|---|---|
| `BE-Mail_x.y.z_x64-setup.exe` | **The installer - this is the one you want** |
| `BE-Mail_x.y.z_x64_en-US.msi` | Alternative installer for managed deployment (Intune/GPO) |
| `latest.json` | Update manifest with the signatures, polled by the built-in updater |

Run the setup. Windows SmartScreen may warn on first install because the installer is not
Authenticode-signed - choose *More info -> Run anyway*. The app installs per user; no
administrator rights required.

On first start BE-Mail asks for the Client ID and Tenant ID of your organisation's Azure app
registration; your administrator has them.

## Updates

BE-Mail checks this repository for updates and installs them itself. Every update is
cryptographically signed and verified before installation, so there is no need to come back
here.

## Terms

BE-Mail is provided **as is**, with no warranty and no support commitment. Making the
installers reachable here does not license anyone to redistribute, mirror or repackage them.

Copyright (c) 2026 Be Interactive. All rights reserved.
