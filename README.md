# Price Monitor

A Windows desktop app that watches product prices on **Hotline.ua** and **E-Katalog** and tells you when they change — in the app, as a Windows notification, or in Telegram.

- See the lowest price for each product, which shop has it, and how it moved in the last 24 hours.
- Price history chart and every current offer across both sites.
- Alerts for price drops, target prices and new all-time lows, with quiet hours.
- English and Ukrainian interface.
- Built-in updates from this repository.

## Download

Get **`Price Monitor Portable vX.Y.Z.exe`** from the [latest release](https://github.com/eclectique/price-monitor/releases/latest).

Requirements: Windows 10 or 11 with Microsoft Edge installed. No Python or installer needed.

## Install

1. Put the EXE in its own folder, for example `C:\Price Monitor\`.
2. Run it. It starts in the system tray; click the tray icon to open the window (Settings → "Start hidden in the tray" turns this off).
3. Paste a product link from Hotline.ua or E-Katalog and press **Add product**.

The app keeps its settings, history and logs in an `app` folder next to the EXE. To move it, copy the EXE together with that folder.

## Updates

Price Monitor checks this repository for new releases **every day** or **every week** (Settings → App updates, or turn it off). When an update is out, the "What's new" window opens once and the tray icon shows an orange dot. Install it with one click; your products, history and settings are kept and backed up first. Downloads are verified against the SHA-256 checksum published with each release.

To verify a download by hand:

```powershell
Get-FileHash ".\Price Monitor Portable v3.3.3.exe" -Algorithm SHA256
```

and compare it with the SHA-256 in the release notes.

## Changes

See [CHANGELOG.md](CHANGELOG.md).
