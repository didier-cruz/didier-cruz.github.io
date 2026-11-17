---
title: Privacy Policy — MoneyTracker
lang: en
---

# Privacy Policy — MoneyTracker

**Controller:** Didier Cruz
**Application:** MoneyTracker (`com.melo.moneytracker`)
**Last updated:** 13 November 2026 (app version 1.6)

---

## Summary

**MoneyTracker does not collect, transmit or share any personal data.**

Everything you record — accounts, movements, categories, goals, budgets,
installment purchases, loans and receipt photos — is stored **only in your device's
private storage**. There is no server to send it
to: the app has no user accounts, requires no sign-up, does not connect to the
internet, and contains no advertising or analytics.

## What data we collect

None.

The app **does not ask for internet access, location, contacts, camera,
microphone, external storage or device identifiers**. The only things it declares
are the **notifications** permission (for the payment reminders you turn on) and
the **phone-startup notice** (so those reminders stay scheduled after a reboot).
Reminders are **local**: they are created and shown on your phone, without
internet, and no data leaves the device. The notifications permission is asked
only when it makes sense and you can refuse it; the app works the same. You can
confirm this yourself under "App permissions" on Google Play, before you even
install it.

When you attach a receipt photo, the app does not use the camera directly: it
asks Android to open **your camera app** or **the system photo picker**, and
receives only the photo you take or choose. The backup works the same way: the
file is saved or opened through **Android's file picker**, in the location you
choose. At no point can the app see your other photos or files.

## What the app stores, and where

The data you enter is held in three places, **all private to the app and on your
own device**:

| What | Where | Contents |
|---|---|---|
| Your finances | Local database `moneytracker.db` | Accounts, starting balances, movements, categories, goals, budgets, installment purchases, loans (rate, installments, insurance and fees), the date of your last backup and your reminder settings (time and reminder types) |
| Scheduled reminders | The app's private storage | The date and text of upcoming reminders, so they can be re-armed if you restart your phone |
| Receipt photos | The app's private folder | Photos you attach to your movements (up to 6 per movement) |
| Your language choice | Local app storage | Only whether you picked Spanish or English |

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

No one. No third parties are involved. The only way your data leaves the app is
if you share a backup file yourself, as described above.

MoneyTracker includes no analytics, crash reporting, advertising, social media or
any other external library that gathers information. No international data
transfer takes place, because no transfer takes place at all.

## How long your data is kept, and how to erase it

Your data stays on your device for as long as you want it there. Since we hold no
remote copy, you have complete control over it:

- **Delete a single item:** remove it from within the app.
- **Delete everything at once:** Android Settings → Apps → MoneyTracker →
  Storage → *Clear data*.
- **Uninstall the app:** Android automatically erases all associated data.

Any of the three is final and irreversible. **We keep no copy**, so there is
nothing to request from us.

**Backup files** you have created are not part of the app: they live wherever you
saved or sent them, and uninstalling the app **does not delete them**. To remove
them, delete them from that folder or service.

## An important warning about your data

Precisely because nothing is sent to the cloud on its own, **if you lose your
device, factory-reset it or uninstall the app, you can only recover your
information if you previously created a backup file and kept it off the phone**.
The app shows the date of your last backup so you know how recent it is.

## Children

MoneyTracker is not specifically directed at children under 13, but it poses no
risk to them either: collecting no data at all, it cannot collect a child's data.

## Your rights

Regulations such as the EU's GDPR and California's CCPA grant you rights of
access, rectification, erasure and portability over your personal data. In
MoneyTracker those rights are satisfied by design: **you already hold all of your
data, on your device, and only you can view, change or delete it.** There is no
request to make of us, because there is nothing of ours to review.

## Changes to this policy

Should a future version of the app change this behaviour — by adding an automatic
cloud backup, for example — this policy will be updated **before** that version
is published, and the change will be stated prominently in the update description
on Google Play.

**History:** 6 November 2026 — added receipt photos (version 1.1), installment
purchases and the backup file with optional password (version 1.2). 13 November
2026 — added loans and local payment reminders, with the notifications and
phone-startup permissions (version 1.6).

## Contact

For any question about this policy, write to:

**didier.cruz.work@gmail.com**

---

*This policy describes the actual behaviour of the published version of
MoneyTracker. Its accuracy can be independently verified by reviewing the
permissions the app declares on Google Play.*
