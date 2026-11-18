---
title: Privacy Policy — MoneyTracker
lang: en
---

# Privacy Policy — MoneyTracker

**Controller:** Didier Cruz
**Application:** MoneyTracker (`com.melo.moneytracker`)
**Last updated:** 18 November 2026 (app version 1.7)

---

## Summary

**Your financial data never leaves your phone.** Everything you record —
accounts, movements, categories, goals, budgets, installment purchases, loans and
receipt photos — is stored **only in your device's private storage**. There is no
server to send it to: the app has no user accounts and requires no sign-up.

**Since version 1.7, the app shows Google AdMob ads** on the Balance and Analysis
screens. To do so it uses the internet, and Google's ads SDK collects some
technical device data (not your finances), as explained below. People who were
already using the app with recorded movements before version 1.7 see no ads, and
for them the app does not contact Google.

## What data we collect

**Financial data: none.** Your amounts, accounts, categories, descriptions and
photos are not sent to anyone, including the ad network. The app does not pass
keywords or screen content to Google to choose ads.

**Data collected by Google's ads SDK** (Google Mobile Ads), automatically, to show
ads, measure them (analytics) and prevent fraud:

| Data | Why |
|---|---|
| IP address, from which the device's **approximate location** can be inferred (city or region, never the precise location) | Choose ads for your area and comply with each country's laws |
| Android **advertising ID** and app set ID | Show relevant ads, cap how often you see the same one and detect fraud |
| **Interactions with ads** (whether they were shown or tapped) and with the app (for example, that it was opened) | Measure ads and pay the developer |
| **Diagnostics** about app and SDK performance | Keep ads working well without wasting battery |

Google receives this data encrypted in transit (TLS) and handles it under its own
policy: [How Google uses information from sites or apps that use our
services](https://policies.google.com/technologies/partner-sites). MoneyTracker's
developer **does not receive this data**: AdMob only shows anonymous totals, such
as how many ads were shown and how much they earned.

**Permissions the app declares:**

- **Internet and network state:** for ads only. Offline, the app works the same
  and shows no ads.
- **Advertising ID** (and Android's Privacy Sandbox ad permissions): for ads, as
  explained above.
- **Notifications:** for the payment reminders you turn on. Asked only when it
  makes sense, and you can refuse it; the app works the same.
- **Phone-startup notice:** so those reminders stay scheduled after a reboot.
  Reminders are **local**: created and shown on your phone, without internet.

The app **does not ask for precise location, contacts, camera, microphone or
external storage**. You can check this under "App permissions" on Google Play.

## Your choices about ads

- **If you live in the European Economic Area, the UK or Switzerland**, the first
  time you open the app you will see Google's consent form. You can accept or
  refuse personalised ads. If you refuse, you will still see ads, but not
  personalised ones. You can change your decision at any time from the side
  menu, under **"Ad privacy"**.
- **In any country** you can reset or delete your advertising ID in Android
  settings (*Settings → Privacy → Ads* or *Google → Ads*, depending on the phone).
  Without an advertising ID, ads are not personalised.
- **We block sensitive categories** in AdMob: dating, "get rich quick" and casino
  games. We also review gambling and cryptocurrency ads and block them when they
  appear.

When you attach a receipt photo, the app does not use the camera directly: it
asks Android to open **your camera app** or **the system photo picker**, and
receives only the photo you take or choose. The backup works the same way: the
file is saved or opened through **Android's file picker**, in the location you
choose. At no point can the app see your other photos or files.

## What the app stores, and where

The data you enter is held in these places, **all private to the app and on your
own device**:

| What | Where | Contents |
|---|---|---|
| Your finances | Local database `moneytracker.db` | Accounts, starting balances, movements, categories, goals, budgets, installment purchases, loans (rate, installments, insurance and fees), the date of your last backup and your reminder settings (time and reminder types) |
| Scheduled reminders | The app's private storage | The date and text of upcoming reminders, so they can be re-armed if you restart your phone |
| Receipt photos | The app's private folder | Photos you attach to your movements (up to 6 per movement) |
| Your language choice | Local app storage | Only whether you picked Spanish or English |
| Your choice about personalised ads | Local app storage (kept by Google's SDK) | Only if you were shown the consent form (Europe, UK, Switzerland) |

That storage is private: Android prevents other apps from reading it. No one else
can access it, and neither can we — we have no technical means to do so, because
the information never leaves your phone.

The app also has Android's automatic backup disabled (`allowBackup="false"`), so
your financial data is not copied to Google's servers either.

## Backing up your data

Since version 1.2 you can create a **backup file** containing all your data and
receipt photos. It works like this:

- **It is only created when you ask for it**, from the Backup screen. The app
  never backs up automatically or sends a backup anywhere on its own.
- **You decide where it goes.** You can save it to a folder on your phone or
  share it with an app of your choice (for example, your email or a cloud storage
  service). From then on the file is subject to the terms and privacy policy of
  **that** app or service, not MoneyTracker's. We never receive a copy.
- **Optional password.** If you turn on "Protect with a password", the file is
  encrypted with AES-256 and cannot be opened without it. The password is not
  stored anywhere: if you forget it, **no one can recover that backup**, us
  included. Without a password, anyone who obtains the file can read its
  contents, so keep it somewhere you trust.
- **Restoring** replaces the app's data with the data in the file you pick. The
  file is read on your phone; nothing is sent to any server.

## Who we share your data with

**Your financial data: no one.** The only way it leaves the app is if you share a
backup file yourself, as described above.

**The technical data in the section above is received by Google** (Google LLC) as
the ad provider, and may be processed on servers outside your country. Google may
share it with the advertisers and ad networks it works with, under its policy
and, in Europe, according to what you accept in the consent form.

MoneyTracker includes no other analytics, crash reporting or social media
services.

## How long your data is kept, and how to erase it

Your data stays on your device for as long as you want it there. Since we hold no
remote copy, you have complete control over it:

- **Delete a single item:** remove it from within the app.
- **Delete everything at once:** Android Settings → Apps → MoneyTracker →
  Storage → *Clear data*.
- **Uninstall the app:** Android automatically erases all associated data.

Any of the three is final and irreversible. **We keep no copy**, so there is
nothing to request from us.

The technical data Google receives for ads is kept and deleted by Google under its
policy. You can reset or delete your advertising ID in Android settings, and
manage your data with Google at [myaccount.google.com](https://myaccount.google.com).

**Backup files** you have created are not part of the app: they live wherever you
saved or sent them, and uninstalling the app **does not delete them**. To remove
them, delete them from that folder or service.

## An important warning about your data

Precisely because nothing is sent to the cloud on its own, **if you lose your
device, factory-reset it or uninstall the app, you can only recover your
information if you previously created a backup file and kept it off the phone**.
The app shows the date of your last backup so you know how recent it is.

## Children

MoneyTracker is not directed at children under 13. We do not knowingly collect
children's data, and the ads are not meant for them.

## Your rights

Regulations such as the EU's GDPR and California's CCPA grant you rights of
access, rectification, erasure and portability over your personal data. In
MoneyTracker those rights are satisfied by design for your financial data: **you
already hold all of it, on your device, and only you can view, change or delete
it.**

For ad data, Google is responsible: you can exercise your rights with Google,
withdraw or change your consent from "Ad privacy" (in Europe) and reset your
advertising ID in Android settings. If in doubt, write to us and we will point
you in the right direction.

## Changes to this policy

Should a future version of the app change this behaviour — by adding an automatic
cloud backup or a new ad network, for example — this policy will be updated **before** that version
is published, and the change will be stated prominently in the update description
on Google Play.

**History:** 6 November 2026 — added receipt photos (version 1.1), installment
purchases and the backup file with optional password (version 1.2). 13 November
2026 — added loans and local payment reminders, with the notifications and
phone-startup permissions (version 1.6). 18 November 2026 — the app shows Google
AdMob ads and, for them only, uses the internet and the advertising ID; your
financial data still never leaves the phone (version 1.7).

## Contact

For any question about this policy, write to:

**didier.cruz.work@gmail.com**

---

*This policy describes the actual behaviour of the published version of
MoneyTracker. The permissions the app declares can be reviewed on Google Play.*
