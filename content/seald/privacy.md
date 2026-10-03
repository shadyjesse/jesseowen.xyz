---
title: "seald — Privacy Policy"
description: "Privacy policy for the seald Android app and web app."
---

**Last updated:** 3 October 2026 (AEST)

**App:** seald  
**Developer / operator:** Jesse Owen  
**Contact:** [jesse@jesseowen.xyz](mailto:jesse@jesseowen.xyz)  
**Delete your account:** [Delete account](/seald/delete-account/)

This policy describes how seald handles information in the Android app and the seald web app. You can use seald as a guest with a local collection. Google Sign-In is optional. Signing in enables free cloud sync.

## 1. What seald is

seald helps you track **sealed** trading-card-game products: barcode scan, on-device collection, catalog search, and market price snapshots. A guest collection stays on the device. If you sign in, the same Google account can use the seald web app for catalog search and, when your collection is synced, for Collection and Insights.

## 2. Data we process

### On your device (local)

- Collection rows (barcode / product id, quantity, optional cost basis, notes)
- Product cache (name, type, game, prices, image URL)
- Recent scan history
- App preferences (filters, display currency, and similar settings)

This is stored in an on-device database. **Guest mode works forever** — no account is required to scan or track a local collection. A guest collection stays on that device unless you export it.

### Camera

- The camera is used **only** to read product barcodes (UPC/EAN and similar) via on-device ML Kit.
- Frames are processed on-device for barcode detection. seald does **not** upload raw camera frames or photos to our servers for scanning. Cloud sync does not include camera frames.

### Optional Google Sign-In

Signing in is optional. If you choose Google Sign-In, we receive a Google ID token and basic profile information (for example your Google subject id and email) and use them to create a seald session. You can keep using the app as a guest without an account.

The same Google account can sign in on the seald web app. Catalog search is available there, and Collection and Insights are available when you are signed in and your collection has been synced.

### Free cloud sync

Signed-in users can sync a collection across devices through the seald API (hosted on Vercel, with data stored in Neon). Sync is free. It is not a paid feature.

Guests stay local-only. We do not upload a guest collection.

Sync stores the collection rows needed to restore your library: product ids, quantities, and optional cost basis and notes where you have entered them. It does not store camera frames or photos.

### Network / catalog

When the Android app or web app talks to the seald API, it may:

- Search or look up sealed catalog entries (product metadata and market price snapshots)
- Load product thumbnails from third-party CDNs (URLs returned by the catalog; typically TCGPlayer CDN hosts)

Server-side catalog ingest uses public/partner sources such as **TCGCSV**. That runs on our servers. The app does not embed partner API secrets.

## 3. What we do not do

- We do **not** sell personal data.
- We do **not** use the camera for advertising, face recognition, or social features.
- We do **not** ship partner API secrets inside the APK.
- We do **not** require an account to scan and track a local collection.
- We do **not** upload raw camera frames or photos for scanning.

## 4. Third parties

| Party | Role |
|---|---|
| Google Play / Android | Distribution and device services |
| Google ML Kit | On-device barcode scanning |
| Google Sign-In | Optional authentication (Google ID token and basic profile) |
| Vercel / Neon | Host the seald API and database for catalog data and signed-in cloud sync |
| Image CDN hosts | Serve product thumbnails referenced by catalog URLs |
| TCGCSV / catalog sources | Server-side sealed product and price snapshots |

## 5. Retention

- **On-device:** until you clear app data or uninstall.
- **Exports you create** (for example CSV): under your control.
- **Cloud:** while your account is active. Synced collection data stays so you can restore it on another device or on the web.

Signing out ends the seald session on that device. It does not, by itself, delete collection data already stored for your account. To delete the Google-linked seald account and the cloud collection synced to it, use the [delete account](/seald/delete-account/) page.

## 6. Children

seald is aimed at adults managing sealed TCG collections. It is not directed at children under 13 (or under 16 where that higher age applies). Do not use seald if you are under the applicable age.

## 7. Your choices

- Deny camera permission — scanning will not work; search and manual entry still can.
- Stay a guest — your collection remains on the device only.
- Sign in with Google — optional. This creates a seald session and enables free cloud sync, including Collection and Insights on the web when your collection is synced.
- Sign out — ends the session on that device. Cloud data already stored for the account remains until you ask us to delete it.
- Clear app storage or uninstall to remove local data.
- Delete your account from the [delete account](/seald/delete-account/) page. Email [jesse@jesseowen.xyz](mailto:jesse@jesseowen.xyz) from the Google account you used to sign in, with the subject "Delete my seald account".

## 8. Changes

We will update this policy when what seald collects or shares changes. Material changes will be reflected at this URL and in the Play listing privacy field.

## 9. Contact

Questions about privacy: [jesse@jesseowen.xyz](mailto:jesse@jesseowen.xyz). To delete your account: [Delete account](/seald/delete-account/).
