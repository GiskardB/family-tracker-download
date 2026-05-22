# Family Tracker — download

> **Official site:** https://giskardb.github.io/family-tracker-download/
> **APK download:** [latest release](https://github.com/GiskardB/family-tracker-download/releases/latest) · sideload only, Android 8+

This repository hosts the **public download page** and the **APK releases** of
Family Tracker. The app's source code lives in a separate repository.

---

## What Family Tracker is

An **open-source**, **non-commercial** Android app that lets a small circle of
trusted family members check in on a loved one — typically an elderly parent or
a relative with a disability — without using any commercial tracking service.

It runs on the **assisted person's** phone and talks **directly** to a private
Telegram bot the family already has on their own phones. No backend, no
separate app for the relatives, no subscription, no cloud account, no data
collected by anyone.

### What it does

- **Real-time Telegram commands** — `/traccia` (GPS), `/foto`, `/audio`, `/stato`
  (battery / signal / last known location), `/tutto` (full check), `/casa`
  (monitored zone), `/trovami` (ring at max volume)
- **Monitored zone (geofence)** — alerts the family if the device leaves a
  configured area during a chosen time window
- **Home-screen widget** — two big always-visible buttons on the Android home
  screen, *"I'm fine"* (green) and *"Help"* (red, with a 5-second cancellable
  SOS). Never opens the app
- **Full transparency** — permanent service notification, visible heads-up
  before every photo/audio capture, and a complete on-device audit log that
  **anyone** using the phone can review at any time
- **Quiet hours & pause** — time windows in which certain commands are blocked;
  manual pause, extendable
- **Security** — bot token stored in the hardware-backed Android Keystore;
  unlock pattern with 12-word BIP39 recovery
- **Multilingual** — Italian and English, live language switching

---

## What's in this repo

| File | Purpose |
|---|---|
| [`index.html`](./index.html) | Public landing page — features, screenshots, commands, download |
| [`telegram-page-home.html`](./telegram-page-home.html) | Telegram WebApp opened by the `/casa` command to configure the monitored zone (address, radius, time window). Bilingual IT/EN |
| `LICENSE` | MIT licence |
| Releases | Signed APKs published automatically from the app's source repo on every release |

The site is published as **GitHub Pages** from the `main` branch. Changes to
`index.html` or `telegram-page-home.html` go live within a few minutes of the
push.

---

## Install

1. Open https://giskardb.github.io/family-tracker-download/ from the **Android
   phone of the assisted person**
2. Download the latest APK
3. Follow the in-app onboarding: create a dedicated Telegram bot, authorise
   family members, grant permissions and (optional) set the unlock pattern

Typical setup time: **about 3 minutes**.

---

## Privacy & responsibility

Family Tracker has no proprietary backend. The app communicates directly with
the Telegram Bot API; **the author has no access to users' data, bots,
locations or media**, and operates no service that retains any user
information.

**Lawful use only.** The app must be installed **exclusively** on a device
whose user has given informed, documented consent (yourself, a minor under
your parental responsibility, or an adult relative who knows and agrees).
Using it to monitor any other person without their knowledge is unlawful in
most jurisdictions — including under the EU GDPR — and is explicitly outside
the intended use of this software.

The author and contributors accept no liability for misuse, missed alerts,
data loss, or any other consequences arising from use of the app. Software
provided "**AS IS**", without warranty of any kind.

Full terms: see the *"Liability · privacy · lawful use"* section at the bottom
of the [landing page](https://giskardb.github.io/family-tracker-download/).

---

## Licence

[MIT](./LICENSE). Non-commercial, designed for family use.

## Trademarks

"Telegram" and "Android" are trademarks of their respective owners, referenced
here only for descriptive purposes. This project is not affiliated with,
endorsed by, or sponsored by any of those entities.
