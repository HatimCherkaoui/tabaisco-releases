# Tabaisco — Releases

This repository contains the official packaged releases of the **Tabaisco** Chrome extension.

> Tabaisco replaces your new-tab page with a fast, focused productivity hub: AI + web search across 12 engines, live weather, rolling news, live sports scores, and a smart app shortcuts panel.

---

## Install

1. Download the latest `.zip` from this repository
2. Unzip it
3. Open Chrome → `chrome://extensions` → Enable **Developer mode**
4. Click **Load unpacked** → select the unzipped folder

Or install directly from the **[Chrome Web Store](#)** _(coming soon)_.

---

## Releases

| Version | Date          | Download                                 | Notes                                                        |
| ------- | ------------- | ---------------------------------------- | ------------------------------------------------------------ |
| v1.0.4 | 31 March 2026 | [tabaisco-1.0.4.zip](tabaisco-1.0.4.zip) | Content script auto-fill for Gemini/Mistral/Copilot, Google Suggest autocomplete, engine scroll throttle |
| v1.0.3 | 31 March 2026 | [tabaisco-1.0.3.zip](tabaisco-1.0.3.zip) | Inline ghost autocomplete and search history |
| v1.0.2  | 29 March 2026 | [tabaisco-1.0.2.zip](tabaisco-1.0.2.zip) | Dropdown fix, remove Minimal light theme                     |
| v1.0.1  | 29 March 2026 | [tabaisco-1.0.1.zip](tabaisco-1.0.1.zip) | Brand icons, keyboard cycling, small-screen alternation, CSP |
| v1.0.0  | 29 March 2026 | [tabaisco-1.0.0.zip](tabaisco-1.0.0.zip) | Initial public release                                       |

### What's new in v1.0.4

- Auto-fill and submit query via content script for Gemini, Mistral, and Copilot
- Inline ghost autocomplete from Google Suggest (Tab to accept, space-aware)
- Search history stored in chrome.storage.local (50 entries, deduplication)
- History dropdown on empty focus with per-entry delete
- Dev proxy routes fetches through localhost:3000 when loaded as extension
- Engine picker scroll throttled to 300ms for smoother UX
- ChatGPT, Claude, Copilot, Grok navigate directly with ?q=

### What's new in v1.0.3

- Inline ghost suggestion via Google Suggest (Tab to accept)
- Search history in chrome.storage.local (50 entries, deduplication)
- History dropdown on empty focus with x delete per entry
- Space-separated queries trigger multi-word completions
- Dev proxy routes ghost fetch through localhost:3000 when running as extension

### What's new in v1.0.2

- **Dropdown fix** — Temperature, news source, and background dropdowns no longer snap shut immediately on click. The engine picker was stealing focus from native `<select>` elements on every outside click.
- **Minimal light theme removed** — The light theme option is gone from the background picker. Any previously saved preference is automatically migrated to Aurora.

### What's new in v1.0.1

- **Brand icons** — Extension icons updated to the full Tabaisco app icon at all sizes.
- **Logo click** — Wordmark fades to low opacity, full on hover; click opens the About tab + donate nudge.
- **Arrow-key engine cycling** — Press `↑`/`↓` in the search bar to switch engines without a mouse.
- **Small-screen news ↔ sports alternation** — On narrow screens (≤ 700 px) the bottom bar alternates between news and sports every 7 s with smooth transitions; both tickers advance in sync.
- **Bug fixes** — Arrow-key double-advance and focus-loss-after-click bugs resolved.
- **CSP hardening** — Explicit `script-src 'self'; object-src 'self'` policy in the manifest. All dynamic `innerHTML` with interpolated variables replaced with safe DOM API calls.
- **Cleanup** — Removed unused `microsoft.png`, corrected SVG filename, fixed Office app URLs, silenced favicon request.

---

## Privacy

See [PRIVACY.md](PRIVACY.md) for the full privacy policy.

**Short version:** Tabaisco collects zero personal data. No analytics, no trackers, no server. Explicit CSP prevents any inline or external script execution.

---

## Source code

The source code is maintained in a private repository.
Contact: cherkaouihatim@gmail.com
