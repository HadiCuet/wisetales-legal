# Wise Tales — Privacy Policy

**Effective date:** June 14, 2026

This policy explains what data Wise Tales collects, why, and the choices you have. Wise Tales is a reading app made for children, so this policy is written in plain English on purpose — parents and guardians should be able to read it in a few minutes.

---

## 1. Who we are

Wise Tales is an iPhone and iPad app for reading bilingual children's folk tales — a side-by-side reader where each sentence shows the source language and the reader's chosen language together, with optional read-aloud narration. It is developed and operated by **Abdullah Al Hadi** ("we", "us"). For the purposes of the EU / UK / EEA General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA/CPRA), Abdullah Al Hadi is the **data controller** for personal data collected through the Wise Tales app. For any privacy questions, contact us at **mukashi.dev@gmail.com**.

---

## 2. Data we collect

### Stays only on your device — never sent anywhere

Everything below is stored locally on your device using Apple's SwiftData framework and iOS user defaults. If you have iCloud Backup enabled, Apple includes this data in your encrypted iCloud backup — that backup is between you and Apple; we have no access to it.

- **Reading progress** — which page of which story you've reached, and which stories you've completed.
- **Preferences** — your settings: reading language, translation language, day/night appearance, and read-to-me options (narration voice, speed, and so on).
- **Purchase status** — whether the one-time "Unlock all tales" purchase has been made on this device.

Uninstalling the app removes all of it.

### Sent to Firebase Analytics (Google)

We use **Firebase Analytics** from Google to understand which tales readers enjoy, so we can decide what to add or improve. It is configured with a children's app in mind — no ads, no advertising identifiers, no cross-app tracking.

**Firebase Analytics** collects:

- A device identifier scoped to this app only (a Firebase installation ID). It cannot identify the reader across other apps, and it resets when the app is reinstalled.
- Device type, OS version, app version, language, and country (derived from IP address).
- Automatic app events — app opens, session starts, and which screens are viewed.
- Two custom story-engagement events, which send **story identifiers only** — never the story text, the sentences, or the translations:
  - **Story opened** — the story's ID, plus the reading language and translation language currently selected.
  - **Story finished** — the story's ID, recorded when the reader reaches the last page.

**We do NOT request App Tracking Transparency permission.** The app does not read your child's advertising identifier (IDFA) — the advertising-identifier component of the analytics SDK is not included in the app, so the IDFA is not accessible to it.

**We never set a user ID.** There is no account, no login, and no persistent identity tied to your child across devices.

**What we do NOT send:** the contents of any story, the sentences or translations the child reads, contact info, payment info, location, photo library content, microphone input, or any name or personal identifier you or your child enters anywhere. The app does not have a microphone, camera, or photo-library permission at all.

### In-app purchases

Wise Tales is free to download, with a few tales free to read and the first page of every other tale free to preview. A single one-time **"Unlock all tales"** purchase removes the lock, through Apple's standard In-App Purchase system (StoreKit 2). The unlock supports Apple **Family Sharing**.

- **Apple processes the payment.** Your payment method (credit card, Apple Cash, etc.) is never seen by the app or by us. Apple charges your Apple ID directly.
- **What the app stores locally:** that the unlock was purchased, which powers the "unlocked" state on this device.
- **We send no purchase, price, receipt, or payment information** to Firebase or anywhere else.
- **Restoring purchases.** If you reinstall the app or use a new device, **Restore Purchases** asks Apple's servers (not ours) which products are tied to your Apple ID and re-unlocks the appropriate content. We don't keep our own purchase database — Apple is the source of truth.

---

## 3. Permissions the app asks for

Wise Tales requests **no special permissions**. It does not access the camera, microphone, photo library, contacts, location, motion data, or notifications. Read-aloud narration uses Apple's on-device speech synthesizer and needs no permission; it can keep playing while the screen is locked (background audio), but this involves no recording and no microphone.

---

## 4. How we use this data

- **Local data** (reading progress, preferences, purchase status) powers the app's features for the reader — picking up where they left off, applying their settings, and unlocking purchased content. It is not used for anything else.
- **Firebase Analytics** tells us, in aggregate, which tales are opened and finished and in which languages — so we can decide which stories and features to add, fix, or improve. We look at aggregate counts, not at individual users.

We do not sell your or your child's personal information, and we do not share it for cross-context behavioral advertising (as those terms are defined under the California Consumer Privacy Act). We do not share data with advertisers, and we do not build profiles across other apps.

---

## 5. Children's privacy (COPPA)

**Wise Tales is directed to children, and we treat all users as if they were under 13.** This affects everything in this policy:

- **No advertising.** The app contains no ads and is not integrated with any ad network.
- **No ad personalization or ad tracking.** The app does not read the advertising identifier (IDFA) and does not request App Tracking Transparency.
- **No persistent user identity.** We do not collect a name, email, phone number, address, photo, or any other directly-identifying information from the child. We never set a user ID. The Firebase installation ID is a per-install random identifier that resets when the app is reinstalled.
- **Erasing data.** Because we don't tie analytics data to an identifiable child, the most reliable erasure is uninstalling the app — which invalidates the Firebase installation ID and removes all local data. Parents and guardians can also email **mukashi.dev@gmail.com** with any access or deletion request.
- **In-app purchases gated by Apple's parental controls.** All purchases go through Apple's standard In-App Purchase flow, so they're subject to whatever parental controls you've configured on the device — including **Ask to Buy** (Family Sharing) and **Screen Time → Content & Privacy Restrictions → iTunes & App Store Purchases**. We do not have a separate purchase flow that bypasses these controls.
- **No data brokers.** The only third party that processes data from this app is Firebase (Google), described in Section 6.

---

## 6. Third parties

The only third-party service the app communicates with is **Firebase**, operated by Google LLC. Google processes Analytics data as our service provider, under the [Firebase Data Processing and Security Terms](https://firebase.google.com/terms/data-processing-terms). Google's own privacy practices are covered by the [Google Privacy Policy](https://policies.google.com/privacy).

Google primarily processes this data on servers located in the **United States**. For users in the EEA, UK, or Switzerland, international transfers rely on Google's Data Processing and Security Terms, which incorporate the European Commission's Standard Contractual Clauses and the UK International Data Transfer Addendum.

No other third-party analytics, advertising, or tracking SDK is bundled in the app.

---

## 7. How long we keep it

- **Local data** — kept on your device until you delete it or uninstall the app.
- **Firebase Analytics** — Google retains event-level data for **14 months** (Firebase's default), after which older events are aggregated or dropped.

---

## 8. Your rights and choices

- **Erase reading data** — uninstalling the app removes all local data and invalidates the Firebase installation ID.
- **Turn off analytics system-wide** — iOS **Settings → Privacy & Security → Analytics & Improvements → Share iPhone Analytics**. You can also prevent all analytics by uninstalling the app.
- **Access or erase your or your child's data** under GDPR (EEA, UK), CCPA/CPRA (California), or similar laws — email **mukashi.dev@gmail.com**. Because we don't tie analytics data to a persistent identity, the most reliable erasure is uninstalling the app, which invalidates the Firebase installation ID.
- **Lodge a complaint** — if you're in the EEA, UK, or Switzerland and believe we're mishandling your data, you have the right to complain to your local data protection authority. We'd appreciate the chance to address your concern first — email **mukashi.dev@gmail.com** and we'll respond within 30 days.

---

## 9. Security

- Local data is stored using iOS's standard app sandbox protections.
- Data sent to Firebase travels over HTTPS (TLS).
- We cannot guarantee perfect security — no one can. If we become aware of a breach that affects your data, we will notify you as required by applicable law.

---

## 10. Changes to this policy

If we change this policy, the new version will replace this page at **https://hadicuet.github.io/wisetales-legal/** and the "Effective date" at the top will be updated. Material changes (e.g. a new third-party service, a new category of data) will be called out in the app's release notes.

---

## 11. Contact us

Questions, requests, or complaints: **mukashi.dev@gmail.com**.
