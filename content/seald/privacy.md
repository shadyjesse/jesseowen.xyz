---
title: "seald — Privacy Policy"
description: "Privacy policy for the seald Android app."
---

**Last updated:** 29 September 2026 (AEST)

**App:** seald  
**Developer / operator:** Jesse Owen  
**Contact:** [jesse@jesseowen.xyz](mailto:jesse@jesseowen.xyz)

This policy describes how the seald Android app handles information. It is written for the current guest-first build and will be updated when Sign-In, cloud sync, or billing ship.

## 1. What seald is

seald helps you track **sealed** trading-card-game products: barcode scan, on-device collection, catalog search, and market price snapshots. Core collection data lives on your device.

## 2. Data we process

### On your device (local)

- Collection rows (barcode / product id, quantity, optional cost basis, notes)
- Product cache (name, type, game, prices, image URL)
- Recent scan history
- App preferences (filters, display currency, and similar settings)

This is stored in an on-device database. **Guest mode works forever** — no account is required to scan or track a local collection. Data stays on the device unless you export it or (in a future version) sign in and enable cloud sync.

### Camera

- The camera is used **only** to read product barcodes (UPC/EAN and similar) via on-device ML Kit.
- Frames are processed on-device for barcode detection. seald does **not** upload raw camera frames or photos to our servers for scanning.

### Network / catalog

When the app talks to the seald API, it may:

- Search or look up sealed catalog entries (product metadata and market price snapshots)
- Load product thumbnails from third-party CDNs (URLs returned by the catalog; typically TCGPlayer CDN hosts)

Server-side catalog ingest uses public/partner sources such as **TCGCSV**. That runs on our servers; the app does not embed partner API secrets.

### Account / Sign-in (not implemented yet)

Google Sign-In is planned. When enabled, we would receive a Google ID token and basic profile info (for example subject id and email) to create a seald session and optionally turn on free cloud sync. Until then, the app runs as a guest.

## 3. What we do not do

- We do **not** sell personal data.
- We do **not** use the camera for advertising, face recognition, or social features.
- We do **not** ship partner API secrets inside the APK.
- We do **not** require an account to scan and track a local collection.

## 4. Third parties

| Party | Role |
|---|---|
| Google Play / Android | Distribution, device services, (future) Play Billing |
| Google ML Kit | On-device barcode scanning |
| Vercel / Neon | Host seald API + database when cloud features are used |
| Image CDN hosts | Serve product thumbnails referenced by catalog URLs |
| TCGCSV / catalog sources | Server-side sealed product + price snapshots |
| Google Sign-In (future) | Authentication |

## 5. Retention

- **On-device:** until you clear app data or uninstall.
- **Exports you create** (for example CSV): under your control.
- **Cloud (future):** while your account is active; deletion steps will be documented when sync ships.

## 6. Children

seald is aimed at adults managing sealed TCG collections. It is not directed at children under 13 (or under 16 where that higher age applies). Do not use the app if you are under the applicable age.

## 7. Your choices

- Deny camera permission — scanning will not work; Search and manual entry still can.
- Stay guest — collection remains local.
- Clear app storage or uninstall to remove local data.
- (Future) Sign out / delete account when cloud accounts exist.

## 8. Changes

We will update this policy when features change (especially Sign-In, sync, or billing). Material changes will be reflected at this URL and in the Play listing privacy field.

## 9. Contact

Questions about privacy: [jesse@jesseowen.xyz](mailto:jesse@jesseowen.xyz)

You can change this contact address later; update this page and the Play Console privacy contact field when you do.
