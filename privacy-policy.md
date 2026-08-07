# Wise Tales — Privacy Policy

**Effective date:** August 7, 2026

This policy explains what data Wise Tales collects, why, and the choices you have. Wise Tales is a reading app made for children, so this policy is written in plain English on purpose — parents and guardians should be able to read it in a few minutes.

---

## 1. Who we are

Wise Tales is an iPhone and iPad app for reading illustrated folk tales to children — one sentence at a time, in a single language chosen from 13, with optional read-aloud narration. The tales themselves work fully offline. It is developed and operated by **Abdullah Al Hadi** ("we", "us"). For the purposes of the EU / UK / EEA General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA/CPRA), Abdullah Al Hadi is the **data controller** for personal data collected through the Wise Tales app. For any privacy questions, contact us at **mukashi.dev@gmail.com**.

---

## 2. Data we collect

### Stays only on your device — never sent anywhere

Everything below is stored locally on your device using Apple's SwiftData framework and iOS user defaults. If you have iCloud Backup enabled, Apple includes this data in your encrypted iCloud backup — that backup is between you and Apple; we have no access to it.

- **Reading progress** — which page of which story you've reached, and which stories you've completed.
- **Preferences** — your settings: the app's language (which sets both the story text and the app's own wording), day/night appearance, and read-to-me options (narration voice, speed, sleep timer, and how words are highlighted).
- **Subscription status** — whether a Wise Tales Plus subscription, or the earlier one-time unlock, is active on this device.
- **App bookkeeping** — which free tales have already been opened (so that a change to the free selection never takes back a tale a child is part-way through), whether the introduction has been seen, and whether the occasional "Enjoying Wise Tales?" prompt and the one-time subscription offer have already appeared.

Uninstalling the app removes all of it.

### Sent to Firebase (Google)

The app uses three Firebase services from Google. Each is described below. All of them are configured with a children's app in mind — no ads, no advertising identifiers, no cross-app tracking.

**Firebase Analytics** helps us understand which tales readers enjoy and whether the subscription screen makes sense, so we can decide what to add or improve. It collects:

- A device identifier scoped to this app only (a Firebase installation ID). It cannot identify the reader across other apps, and it resets when the app is reinstalled.
- Device type, OS version, app version, language, and country (derived from IP address).
- Automatic app events — app opens, session starts, and which screens are viewed.
- A small set of custom events, which send **identifiers and counts only** — never the story text, and never any payment detail:
  - **Story opened** — the story's ID and the language it's being read in.
  - **Story finished** — the story's ID, recorded when the reader reaches the last page.
  - **Subscription screen shown / dismissed** — what raised the screen (for example: the introduction, a locked tale, the settings page), how many seconds it stayed open, and which plan was highlighted when it closed.
  - **Purchase started / purchase result** — which plan was chosen (monthly or yearly), and how Apple's payment sheet resolved (completed, cancelled, or pending).

**Firebase Cloud Messaging** delivers the app's occasional notifications — a new tale has arrived, and now and then a note about Wise Tales Plus.

- **We store no device tokens** — not on your device, not on a server. We have no user database.
- Every message is addressed to a **topic**, not to a person. Your device joins at most two: one for the language the app is set to, and — only while the library is still locked — one for readers who haven't subscribed. That membership tells Google's delivery service the app's language and whether the tales are unlocked, and nothing else. It says nothing about which tales are read.
- Because we send to topics, **we cannot target an individual reader.** Everyone on a topic gets the same message.
- To deliver a notification at all, Google issues a registration token for this app installation. It is per-install and resets when the app is reinstalled.
- Notifications are optional — see Section 3.

**Firebase Remote Config** tells the app which tales are currently free to read. At launch the app asks Firebase for that list; the request carries the installation ID and standard device information, and **no reading data**. If the request fails, the list built into the app is used instead — so the app works the same with no network at all.

**We do NOT request App Tracking Transparency permission.** The app does not read your child's advertising identifier (IDFA) — the advertising-identifier component of the analytics SDK is not included in the app, so the IDFA is not accessible to it.

**We never set a user ID.** There is no account and no login. The identifiers described above are per-installation and random; they are not tied to a name, an email, or an Apple ID, and they reset when the app is reinstalled.

**What we do NOT send:** the contents of any story, the sentences the child reads, contact info, payment info, receipts, prices, Apple ID details, location, photo library content, microphone input, or any name or personal identifier. The app does not have a microphone, camera, or photo-library permission at all.

### Subscriptions and purchases

Wise Tales is free to download. A selection of tales is free to read in full, and every other tale's first page is free to preview.

**Wise Tales Plus** opens the whole library. It is an auto-renewing subscription — **monthly or yearly** — sold through Apple's standard In-App Purchase system (StoreKit 2). It renews until it is cancelled, and it can be cancelled at any time in **Settings → your Apple Account → Subscriptions** on your device.

Readers who bought the earlier one-time **"Unlock all tales"** purchase keep full access permanently, at no further cost. That product is no longer sold, but it is still honoured.

- **Apple processes the payment.** Your payment method (credit card, Apple Cash, etc.) is never seen by the app or by us. Apple charges your Apple Account directly.
- **What the app stores locally:** whether access is currently active, which powers the "unlocked" state on this device.
- **We send no price, receipt, or payment information** to Firebase or anywhere else. The purchase events described above record only which plan was chosen and whether Apple's sheet completed.
- **Restoring purchases.** If you reinstall the app or use a new device, **Restore Purchases** asks Apple's servers (not ours) what is tied to your Apple Account and restores access. We don't keep our own purchase database — Apple is the source of truth.
- **Refunds** are handled by Apple, at [reportaproblem.apple.com](https://reportaproblem.apple.com).

---

## 3. Permissions the app asks for

**Notifications are the only permission Wise Tales asks for.** During the app's introduction it explains what the notifications are for and then lets iOS ask your permission. Declining changes nothing else about the app — every tale, the narration, and the settings all work exactly the same. You can change your mind at any time in **iOS Settings → Notifications → Wise Tales**, or turn notifications off there entirely.

The app does **not** access the camera, microphone, photo library, contacts, location, or motion data. Read-aloud narration uses Apple's on-device speech synthesizer and needs no permission; it can keep playing while the screen is locked (background audio), but this involves no recording and no microphone.

---

## 4. How we use this data

- **Local data** (reading progress, preferences, subscription status, app bookkeeping) powers the app's features for the reader — picking up where they left off, applying their settings, and unlocking subscribed content. It is not used for anything else.
- **Firebase Analytics** tells us, in aggregate, which tales are opened and finished and in which languages, and whether readers understand the subscription screen — so we can decide which stories and features to add, fix, or improve. We look at aggregate counts, not at individual users.
- **Firebase Cloud Messaging** lets us tell readers about a new tale in their own language, and occasionally about Wise Tales Plus.
- **Firebase Remote Config** lets us change which tales are free without shipping an app update.

We do not sell your or your child's personal information, and we do not share it for cross-context behavioral advertising (as those terms are defined under the California Consumer Privacy Act). We do not share data with advertisers, and we do not build profiles across other apps.

---

## 5. Children's privacy (COPPA)

**Wise Tales is directed to children, and we treat all users as if they were under 13.** This affects everything in this policy:

- **No advertising.** The app contains no ads and is not integrated with any ad network.
- **No ad personalization or ad tracking.** The app does not read the advertising identifier (IDFA) and does not request App Tracking Transparency.
- **No account and no persistent identity for the child.** We do not collect a name, email, phone number, address, photo, or any other directly-identifying information. We never set a user ID. The Firebase installation ID and the notification registration token are per-install random identifiers that reset when the app is reinstalled.
- **Notifications are opt-in and adult-controlled.** They only arrive if someone grants the iOS permission prompt, they are infrequent, and some of them mention Wise Tales Plus. Because every message is sent to a whole language topic, no child can be singled out or targeted individually. Notifications can be switched off at any time in **iOS Settings → Notifications → Wise Tales**.
- **Erasing data.** Because we don't tie analytics data to an identifiable child, the most reliable erasure is uninstalling the app — which invalidates the Firebase installation ID and the notification token and removes all local data. Parents and guardians can also email **mukashi.dev@gmail.com** with any access or deletion request.
- **Purchases gated by Apple's parental controls.** All purchases and subscriptions go through Apple's standard In-App Purchase flow, so they're subject to whatever parental controls you've configured on the device — including **Ask to Buy** (Family Sharing) and **Screen Time → Content & Privacy Restrictions → iTunes & App Store Purchases**. We do not have a separate purchase flow that bypasses these controls.
- **No data brokers.** The only third party that processes data from this app is Firebase (Google), described in Section 6.

---

## 6. Third parties

The only third-party service the app communicates with is **Firebase**, operated by Google LLC — specifically Firebase Analytics, Firebase Cloud Messaging, and Firebase Remote Config. Google processes this data as our service provider, under the [Firebase Data Processing and Security Terms](https://firebase.google.com/terms/data-processing-terms). Google's own privacy practices are covered by the [Google Privacy Policy](https://policies.google.com/privacy). Notifications are delivered to your device through **Apple Push Notification service**, which is operated by Apple.

Google primarily processes this data on servers located in the **United States**. For users in the EEA, UK, or Switzerland, international transfers rely on Google's Data Processing and Security Terms, which incorporate the European Commission's Standard Contractual Clauses and the UK International Data Transfer Addendum.

No other third-party analytics, advertising, or tracking SDK is bundled in the app.

---

## 7. How long we keep it

- **Local data** — kept on your device until you delete it or uninstall the app.
- **Firebase Analytics** — Google retains event-level data for **14 months** (Firebase's default), after which older events are aggregated or dropped.
- **Notification topic membership** — kept by Firebase for as long as the app is installed. It changes when you change the app's language or subscribe, and it is released when the app is uninstalled.
- **We hold nothing on a server of our own.** There is no Wise Tales account database, purchase database, or device-token database to retain.

---

## 8. Your rights and choices

- **Erase reading data** — uninstalling the app removes all local data and invalidates the Firebase installation ID and notification token.
- **Turn off notifications** — **iOS Settings → Notifications → Wise Tales**. Nothing else in the app changes.
- **Cancel a subscription** — **Settings → your Apple Account → Subscriptions** on your device. Cancelling stops the renewal; access continues until the paid period ends.
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

**What changed on August 7, 2026:** the app became monolingual — one chosen language for both the story and the app itself, with the side-by-side translation reader removed; the one-time "Unlock all tales" purchase was replaced by the Wise Tales Plus monthly and yearly subscriptions (the old unlock is still honoured); optional push notifications were added through Firebase Cloud Messaging; Firebase Remote Config was added to manage which tales are free; and the analytics section now also describes the subscription-screen and purchase events.

---

## 11. Contact us

Questions, requests, or complaints: **mukashi.dev@gmail.com**.
