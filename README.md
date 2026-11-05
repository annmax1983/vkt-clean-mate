# VKT CleanMate

English | [中文](languages/README_zh.md) | [日本語](languages/README_ja.md) | [Deutsch](languages/README_de.md) | [Español](languages/README_es.md) | [Français](languages/README_fr.md)

**Preview-first browsing data cleaner.** See exactly what will be deleted before it is deleted, keep the domains you trust untouched, and find out where your focus time actually goes.

> Chrome · Edge · Firefox · Manifest V3 · Minimal permissions · Local only

Part of the [VKT](https://www.annmax1983.com/) privacy-first toolkit.

---

## Why VKT CleanMate?

Most cleaners are one big "wipe everything" button. That is exactly why people are afraid to turn them on: one click and every login is gone.

VKT CleanMate separates the decision from the action:

1. **Preview before deleting** — a summary of what will be removed (site count, history entries, cookies, data types, retention) is shown before each manual run; scheduled runs follow your rules and notify you when done.
2. **Targeted mode is free** — only the domains on your clean list are wiped. Everything else is never touched, so a free user has no way to lose data by accident.
3. **Protected list** — in Full mode the domains you protect are skipped, so you stay signed in where it matters.
4. **Focus footprint** — tracks how long you actually *watch* a site (not how many tabs you opened), then tells you which domains are worth cleaning. It exists to feed the cleaner, not to be a second product.

| What other cleaners do | The cost |
|---|---|
| One switch that wipes everything | One mis-click and every session, cookie and download record is gone |
| A confirmation dialog with no numbers | You cannot tell whether this cleans 3 sites or 3000 before you commit |
| Site rules hidden behind a regex field | Nobody writes them, so the "safe" mode never actually gets used |

| What VKT CleanMate does | The result |
|---|---|
| **Preview sheet on every manual run** | Real counts from the browser: sites found, history entries, cookies, active data types, retention window |
| **Free tier cannot run a full wipe** | A free user has no path to accidental data loss — by design, not by warning |
| **Two lists pointing in opposite directions** | Clean list ("only these") and protected list ("never these") — both free, and protection wins in either mode |
| **Honest limits written down** | In the interface and in this README, rather than discovered by a reviewer |

---

## Features

### 🆓 Free, forever

| Feature | What it does |
|---|---|
| Preview sheet | Sites found, history entries, cookies, data types and retention, before anything is removed |
| Targeted mode | Cleans only the domains on your clean list. Unlimited entries |
| Protected list | Domains that are never touched. Protection wins over the clean list, in both modes |
| Nine data types | History, cache, cookies, download history, form data, local storage, IndexedDB, service workers, saved passwords — each a separate switch |
| Retention | Keep the last 1 day / 3 days / 7 days / 30 days, or everything |
| Five triggers | On startup, on browser close, every N minutes, daily at a chosen time, after N minutes idle |
| Per-trigger scope | e.g. history + cache every few hours, a deep clean including cookies when the browser closes |
| Shortcuts | `Alt+Shift+C` clean now · `Alt+Shift+X` clean + close all tabs |
| Snooze | Push the next automatic run back by one hour |
| Notifications | A result summary after every run |
| Run log | The last 12 runs with time, trigger, sites and entries removed |
| Right-click actions | Add the current site to the clean list, protect it, or open the preview for it |
| Focus footprint | Real focus time per domain, 24-hour histogram, ranking, "worth cleaning" suggestions, CSV export — recording starts while the footprint page is open |
| Six languages | English, 简体中文, 日本語, Deutsch, Español, Français |

### ⭐ Pro (licence required)

| Feature | What it does |
|---|---|
| Full mode | Clean everything except your protected list |
| Background recording | Keep collecting focus time after the footprint page is closed, instead of only while it is open |
| 30-day trend | Daily focus time for the last 30 days, plus this week against last week |

A licence covers two browsers. The free features keep working after a licence expires.

---

## What it can and cannot do

### ✅ It can

- Wipe history, cache, cookies, downloads, form data, local storage, IndexedDB, service workers and passwords, in any combination.
- Restrict a cleanup to the domains you named — matching the domain and its subdomains, with no regex.
- Skip the domains you protect, in Full mode.
- Clean on a schedule, with a different data scope per trigger.
- Report exactly what was removed, every time.

### ❌ It cannot

- Clear DNS caches, router logs, ISP records or server-side logs. Those are not on your device.
- Restore deleted history. Chromium has no API to write history back, for any extension.
- Clean another browser's data, another profile, or a synced copy on another device.
- Limit history, downloads, form data or passwords to a single site. The browser does not expose that; those four are filtered only in Full mode, and the interface says so next to the checkbox.
- Guarantee the "on browser close" trigger. It is best-effort: a crash, a forced restart or a power cut can lose that one run.
- Clean what was never stored. A page you only read in a private window leaves nothing behind.
- Replace a VPN or defend you against network-level monitoring. It is a self-service tool for your own browser on your own device.

---

## Preview

> 📸 Store assets and screenshots live in [`screenshots/`](screenshots/) — five 1280×800 shots plus a 1400×560 and a 440×280 promo tile.

| Screenshot | What it shows |
|---|---|
| [`01-popup.png`](screenshots/01-popup.png) | Toolbar popup, current site already in the clean list |
| [`02-preview.png`](screenshots/02-preview.png) | The "Before cleaning" confirmation sheet |
| [`03-cleaning.png`](screenshots/03-cleaning.png) | Settings — cleaning mode, data types, retention, triggers |
| [`04-lists.png`](screenshots/04-lists.png) | Settings — clean list and protected list |
| [`05-footprint.png`](screenshots/05-footprint.png) | Footprint page — totals, hour histogram, ranking |

---

## Supported Browsers

| Browser | Status |
|---|---|
| Chrome 116+ (desktop) | ✅ Supported |
| Microsoft Edge 116+ (desktop) | ✅ Supported |
| Chromium-based browsers with MV3 | ✅ Should work |
| Firefox (desktop) | ✅ Supported |
| Mobile / tablet | ❌ Not supported — there is no toolbar to click |
| Private windows | ⚠️ Nothing to clean: data is discarded when the window closes |

---

## Install

| Store | Link |
|---|---|
| Chrome Web Store | — not published yet (use Edge or Firefox) |
| Microsoft Edge Add-ons | [Install for Edge](https://microsoftedge.microsoft.com/addons/detail/amfipoeaanhnmhhcfcfdngffnhmgjjfb) |
| Firefox Add-ons (AMO) | [Install for Firefox](https://addons.mozilla.org/firefox/addon/vkt-cleanmate/) |

> Install only from the official stores above — avoid third-party download sites.

**From source:**

```bash
npm install          # terser, only for the build
npm run build        # dist/ + publish/cleanmate-v<version>.zip
```

Then `chrome://extensions` → Developer mode → Load unpacked → this folder (or the unpacked `dist/`).

---

## Usage

### First run

Open the popup and press **Clean now**. Because the default mode is Targeted and the clean list is empty, nothing happens yet — that is the point. Add a domain first, in the popup for the current site, or on the **Lists** tab.

### Filling the clean list

- In the popup: **Add current site** adds the domain you are looking at.
- On the Lists tab: type `example.com` and press Add. Subdomains are covered automatically; `www.` is stripped for you.
- On the Footprint page: the "worth cleaning" suggestions and the ranking rows both have a button that adds the domain.

### Configuring automatic runs

On the **Cleaning** tab each of the five triggers has a switch. Below it, a dropdown sets that trigger's data scope — `global` uses the checkboxes above, any other value restricts that run to a preset (history + cache, cookies + cache, everything, and so on).

A reasonable starting point: history + cache every 6 hours, everything when the browser closes, and leave startup and idle off until you know you want them.

### Shortcuts

| Keys | Action |
|---|---|
| `Alt+Shift+C` | Clean now, using the current settings |
| `Alt+Shift+X` | Clean now, then close every tab and window |

Both can be rebound at `chrome://extensions/shortcuts`.

---

## How it works

1. A trigger fires, or you press Clean now.
2. The background service worker resolves the domain scope: your clean list in Targeted mode, everything minus the protected list in Full mode.
3. On a manual run it counts what would be affected — sites, history entries, cookies — and shows the preview sheet before touching anything. **Nothing is deleted until you confirm.**
4. On confirm, each selected data type is removed through `chrome.browsingData`, in batches of at most 50 origins. A scheduled run (interval, daily, idle, on-close) skips the sheet — it executes the rules you configured and reports the result by notification.
5. Domain rules are expanded to real origins first — `browsingData` accepts origins (`https://example.com`) rather than bare hosts, and does not expand subdomains itself.
6. A notification reports the result, the last-run timestamp is stored, and the sheet stays reachable from the popup.

One implementation detail worth knowing: `browsingData` only honours `origins` for cache, cookies, local storage, IndexedDB, service workers and file systems. History, downloads, form data and passwords ignore the origin list entirely — so when those types are selected, the run covers the whole profile. The extension says so in the interface instead of pretending otherwise.

---

## FAQ

**Will cleaning delete my bookmarks?**
No. Bookmarks are not part of `browsingData`, and nothing in the extension touches them.

**Will cleaning cookies sign me out everywhere?**
In Targeted mode, only for the domains you listed. That is why the free tier runs only in Targeted mode: a full wipe is a paid decision, made deliberately, with a protected list in hand.

**Can I clean history for one site only?**
Yes. That needs the optional `history` permission, which is requested at the moment you preview or clean history per site — not at install.

**Does it delete the passwords synced to my Google account?**
If you tick **Saved passwords**, the browser deletes the local password store, and a signed-in profile can propagate that deletion. The type is off by default and marked in red in the interface for exactly this reason. Leave it off unless you mean it.

**Does it work in private windows?**
A private window discards its own data when it closes, so there is nothing left to clean. The extension does not need access to private windows.

**The "on browser close" trigger did not run.**
It is best-effort. The extension fires when the window count reaches zero, and if the browser exits mid-task the cleanup finishes a few seconds after the next start. A crash, a forced restart or a power cut loses that run.

**Does it clean other browsers or other profiles?**
No. One profile, one browser, this device.

**Why is only Full mode paid?**
Because a full wipe is the one operation that can remove logins you still need. It is also the only thing a targeted cleaner structurally cannot do — everything else here, including the protected list and the footprint data, works without a licence. Pro adds the risky operation and the long-term recording, not the ability to look at your own data.

---

## Privacy

No analytics, no telemetry, no ads, no account. The extension does not read page content, does not record keystrokes and does not build a profile. Settings live in `chrome.storage.local`. The focus footprint, if enabled, stores domains, durations, visit counts and an hour histogram in a 30-day rolling window — no URLs, no titles. The only network request in the entire extension is licence verification against `api.annmax1983.com`, and only if you paste a key.

**[📄 Full Privacy Policy](privacy-policy.html)**

### Permissions

| Permission | Why |
|---|---|
| `browsingData` | Delete the data types you selected |
| `storage` | Keep settings and the optional footprint on your device |
| `alarms` | Schedules, plus a one-minute heartbeat for focus timing |
| `tabs` | Know the current domain and act on the visible tab |
| `windows` | Detect the last window closing — the "on browser close" trigger |
| `idle` | The optional "after idle" trigger |
| `notifications` | The result summary after a run |
| `contextMenus` | The right-click entries: add to the clean list, protect this site, preview this site |
| `history` *(optional)* | Only requested when you preview or clean history per site |
| `cookies` *(optional)* | Only requested when you clean cookies per site |
| `api.annmax1983.com` | Licence activation and validation only |

The optional pair is the reason a fresh install does not show the red "read your browsing history" warning.

---

## Development

```bash
npm install                   # terser, only for the build
npm run icons                 # regenerate icons/*.png (no dependencies)
npm run build                 # dist/ + publish/cleanmate-v<version>.zip
npm run shoot                 # regenerate screenshots/ at store sizes
node tools/check-locales.js   # verify all six locales share the same key set
```

Load unpacked: `chrome://extensions` → Developer mode → Load unpacked → this folder.

### Project layout

```
manifest.json          MV3, service_worker as ES module
background.js          scheduling, rule engine, clean executor, focus tracking
license.js             Creem licence (plugin id: cleanmate)
common/                store (defaults/merge), domain matching, i18n, formatters, ui.css
popup/                 one-click clean + preview sheet + current-site actions
options/               mode, data types, triggers, lists, footprint switch, licence
insights/              Footprint page — free to view; collection runs while this page is open (always-on is Pro)
_locales/              en, zh_CN, ja, de, es, fr (174 keys each)
languages/             translated READMEs (zh, ja, de, es, fr)
assets/                shared UI icons (GitHub / coffee / favicon)
store-listing/         store copy for all six languages
index.html             landing page (not shipped in the extension zip)
promo.html             store promo tile (screenshot target) — 1400×560, `?size=small` gives 440×280
screenshots/           store screenshots, regenerated by `npm run shoot`
tools/make-icons.js    dependency-free PNG icon generator
tools/check-locales.js verifies all locales share the same key set
tools/shoot.js         renders every surface to screenshots/ at store sizes
tools/harness/         mock chrome.* + a fake page, used only by tools/shoot.js
```

### Store screenshots

`npm run shoot` regenerates everything in `screenshots/` at the exact store sizes:

| File | Size | What it shows |
|---|---|---|
| `01-popup.png` | 1280×800 | toolbar popup, current site already in the clean list |
| `02-preview.png` | 1280×800 | the "Before cleaning" confirmation sheet |
| `03-cleaning.png` | 1280×800 | settings — cleaning mode, data types, retention, triggers |
| `04-lists.png` | 1280×800 | settings — clean list and protected list |
| `05-footprint.png` | 1280×800 | Footprint page — totals, hour histogram, ranking |
| `promo.png` | 1400×560 | promo tile |
| `promo-small.png` | 440×280 | small promo tile |

The runner needs Chrome/Edge and `puppeteer-core` (it looks in `node_modules`, then in the
sibling extension repos). It does not install the extension: `tools/harness/server.js` serves the
real `popup/`, `options/` and `insights/` pages with a mock `chrome.*` injected into `<head>`,
so the UI renders with seeded data. Chrome 137+ removed `--load-extension`, so this is the only
way to get reproducible shots without a manual capture.

The upload set is `01`–`05` plus the two promo tiles. The store accepts **at most 5
screenshots**, so those five are already the full allowance. `landing.png` is a leftover
capture of `index.html` and is not a store asset.

### Notes on the focus tracker

- Off by default. Viewing the footprint, the ranking, the suggestions and the CSV export are free; background recording and the 30-day trend are Pro.
- Default mode records **only while the Footprint page is open** (a long-lived port keeps it alive). Closing the page stops recording. "Always" keeps it running in the background and is part of Pro.
- The service worker cannot use `setInterval` — sessions are committed on tab/window events and flushed by a 1-minute alarm. A flush only writes the current block; the session continues, so a heartbeat never counts as a new visit.
- Only counted while the tab is active **and** its window is focused and not minimised. Ten minutes without any input is treated as "away" and stops counting; a single block is capped at five minutes, so a sleep or a laptop lid closing cannot turn eight idle hours into eight hours of "focus".
- Only `domain`, `duration`, `visits` and an hour histogram are stored. No URLs, no titles.
- A free user who never opens the page records nothing at all, and the daily trend is not sent to the page for them — the paid gate sits in the background, not in the DOM.

---

## 中文说明

**在做的事**：一个"先看清再删"的浏览数据清理器。免费版只清「清理名单」里的域名，永远不会误伤其它数据；付费版多一个"清全部"和长期记录。

**核心差异**：
1. 清理前必出预览（命中站点数、历史条数、Cookie 数、保留期）
2. 「专注足迹」只统计你真正在看的时长，而不是开了多少标签页，并给出"该清哪个"的建议——数据、排行、建议和 CSV 都免费
3. 统计默认关闭，且默认只在足迹页面打开时采集；付费买的是"关掉页面继续记录"和 30 天趋势
4. 保护名单免费，且两种模式下都生效（保护优先于清理）

**故意的取舍**：不做正则规则、不做锁屏触发。

---

## Copyright Disclaimer

VKT CleanMate is an independent tool. It is not affiliated with Google, Microsoft or any browser vendor. Chrome, Edge and Firefox are trademarks of their respective owners.

The extension deletes data through the browser's own APIs. It does not patch the browser, does not modify system files and does not install anything outside its own extension folder.

---

## Source Code Notice

The published package contains readable JavaScript — no obfuscation. `dist/` is the built, minified output; the source in this repository is what the build consumes. Nothing is loaded remotely: the extension has no `eval`, no remote scripts and no dynamic imports outside its own package, which is enforced by the MV3 content security policy in `manifest.json`.

---

## ❤️ Support

**[👉 Get a licence key](https://annmax1983.com/extensions/cleanmate)** · **[☕ Buy me a coffee](https://ko-fi.com/annmax?ref=vkt-clean-mate)** · [Source on GitHub](https://github.com/annmax1983/vkt-clean-mate) · [Official website](https://annmax1983.com/)

---

## License

Copyright © 2026 VKT CleanMate. All rights reserved.

---

## Links

- **Official website:** https://annmax1983.com/
- **This extension:** https://annmax1983.com/extensions/cleanmate
- **Privacy policy:** https://annmax1983.com/privacy
- **Contact:** support@annmax1983.com
- **☕ Support this project (Ko-fi):** https://ko-fi.com/annmax?ref=vkt-clean-mate
