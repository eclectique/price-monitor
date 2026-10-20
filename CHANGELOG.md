# Changelog

## 3.3.0 — 2026-10-20

Lighter on weak PCs, smoother switches.

- Faster, lighter price checks: one browser is shared by all sources of a check, and pages load without images, fonts, ads and third-party trackers ("Don't load images", on by default). Measured on 2 products × 2 sites: check time 29.9 s → 18.6 s, browser CPU −58%, peak browser memory 885 MB → 502 MB — same prices found. If a site fails in light mode, the retry loads the page fully.
- Almost no CPU while in the tray: the hidden window no longer re-reads the log or redraws (idle CPU −96%).
- The log file rotates at 2 MB; price and alert history are read incrementally; product search waits until you stop typing.
- Smaller, smoother on/off switches with hover and focus states.

## 3.2.0 — 2026-10-20

Built-in updates.

- The app checks for new versions on its own, **every day** or **every week** (Settings → App updates; can be turned off). The check is one request to GitHub and never interrupts a price check.
- When a new version is out, a banner appears with **What's new & update**: read the release notes, then **Update now**, **Skip this version** or close.
- **Update now** downloads the new EXE from GitHub, verifies its size and SHA-256 checksum, backs up your data, replaces the program file in place (autostart keeps working) and restarts. Products, price history and settings are kept.
- Optional **Install updates automatically** does the same unattended, waiting until no price check is running.
- Updates come only from github.com/eclectique/price-monitor over HTTPS; files without a matching checksum are refused.
- The previous manifest/ZIP update mechanism has been removed.

## 3.1.0 — 2026-10-20

New main window. Monitoring, Telegram and settings behaviour is unchanged.

- Sidebar navigation (Products · Alerts & activity · Settings) with a live status card: monitoring state, countdown to the next check, last success.
- Products: summary tiles, a clear "Track a new product" box, filters (All / Changed in 24h / Needs attention), search and folders. Each product shows the lowest price, where it is, the 24-hour change, a plain-language status and the last check time.
- Product details (double-click a product): lowest price and shop, 24-hour change, lowest-ever price, target price, a Hotline vs E-Katalog price chart, every current offer across both sites, source health, and the alert rules in plain words.
- Alerts & activity: every Telegram alert in plain language with copy / send again, plus the technical log and "Copy diagnostics".
- Settings: grouped cards with switches. A banner reminds you to save unsaved changes.
- New light theme for all windows and dialogs. The window is freely resizable; F11 toggles fullscreen.
