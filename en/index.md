# Privacy Policy — Kiosq

**Last updated: May 4, 2026**

This policy describes how the **Kiosq** application ("the App", published
by Gaïalabx) handles your data. By using Kiosq, you accept the practices
described below.

Our principle: **your data belongs to you**. Kiosq works mostly offline,
without ads, without tracking, and without sending your reading
behavior to third parties.

## 1. Data stored locally on your device

The App locally stores (Hive database, sandboxed by Android):

- Your configured RSS feeds / video channels / podcasts
- Your categories, subjects (alert keywords) and favorites
- Article history downloaded (purged according to your setting,
  30 days by default)
- Your display and reading preferences
- Your reading statistics (articles read, daily streak)
- Podcast playback progress
- Cached images and content for offline reading

This data **never** leaves your device unless you explicitly enable
cloud backup (see section 2).

## 2. Google Drive cloud backup (optional)

If you enable cloud backup, the App:

- Authenticates your Google account via OAuth (token stored only on
  your device)
- Backs up your configuration (feeds, categories, subjects, settings)
  to the **Kiosq-restricted folder** of your personal Google Drive.
  No other folder is accessible.
- Allows restoration on a new device

Your data **never** transits through our servers: communication is
direct between your device and Google Drive's API. You retain ownership
and access control via your Google account.

To revoke access: Kiosq Settings → Sync, or via
[myaccount.google.com](https://myaccount.google.com/permissions).

## 3. Anonymous crash reports (Firebase Crashlytics)

To improve stability, the App may **automatically** send technical
reports in case of a crash. These reports contain:

- The technical crash trace (stack trace)
- The App version and Android version
- Your device model
- Your system language
- An **anonymous and local** identifier (UUID generated on your device,
  not linked to your identity, account, or phone number)

**No personal data, no article content, and no reading behavior is sent.**

This service is provided by Firebase Crashlytics (Google). Google's
policy: [policies.google.com/privacy](https://policies.google.com/privacy).

**You can disable this collection at any time** in
Settings → General → Privacy → Crash reports.

## 4. Article translation service (on demand)

When you tap "Translate" on an article, the article text is sent to
Google Translate's public API (`translate.googleapis.com`) for
translation. No user identifier is attached to the request.

This communication only occurs on **explicit tap**. No text is sent
in the background.

## 5. Web page rendering (WebView)

For "Web" reading mode of an article, the App loads the article's
original page in an Android WebView component. The remote site may
then set its own cookies, analytics, or ads (practices specific to
each publisher). These cookies are isolated from your main browser
and can be cleared via Android system settings.

## 6. In-app purchases (donations)

If you make a donation to support the App, the transaction is fully
handled by Google Play Billing. We receive **no banking data**, only
the confirmation that the transaction succeeded.

## 7. Notifications

Notifications (new articles, Subject alerts) are **generated locally**
by your device. They require no external push server. You can disable
them via Kiosq Settings or Android system settings.

## 8. Data we do NOT collect

The App **does not collect or transmit**:

- Your location
- Your contacts, calendar, SMS, photos, microphone, camera
- Your advertising identifier (Advertising ID)
- Your browsing history
- Your reading behaviors (which articles, at what time, etc.)
- Your favorites for commercial purposes

No ads are displayed. No tracking pixel is integrated.

## 9. Android permissions requested

| Permission | Purpose |
|---|---|
| Internet access | RSS feed synchronization |
| Network state | Wi-Fi vs cellular detection ("Wi-Fi only sync" option) |
| Notifications (Android 13+) | New article alerts |
| Foreground service | Podcast audio playback |
| Wake lock | Keep audio playback active |
| Auto-start | Resume sync tasks after restart |
| Vibrate | Notifications |
| In-app billing | Donations |

## 10. Data retention

- Local data: kept as long as the App is installed. Complete deletion
  via uninstall or Settings → Data → Reset.
- Cloud backup: kept as long as you wish. Deletion via Settings → Sync
  → Delete cloud backup.
- Crash reports: kept 90 days by Firebase Crashlytics, then automatically
  deleted.

## 11. Your rights (GDPR)

In accordance with GDPR, you have the following rights:

- **Access**: all your data is visible within the App itself.
- **Rectification**: modify your settings directly in the App.
- **Deletion**: uninstall the App, or delete the cloud backup, or
  disable Crashlytics.
- **Portability**: export your feeds in OPML format via Settings →
  Data → Export.
- **Objection**: disable Crashlytics (Settings → Privacy) or cloud
  sync at any time.

For any data-related question: kiosqrssatm@gmail.com.

## 12. Children

The App is not intended for children under 13 and does not knowingly
collect any data from children. If you are a parent and believe your
child has provided data, contact us for deletion.

## 13. Security

Your local data is stored in the App's sandbox (Android-reserved area).
Network communications use HTTPS. Cloud backup transits directly between
your device and Google Drive, with no intermediate server.

Since no system is foolproof, we cannot guarantee absolute security,
but we apply industry-standard practices.

## 14. Changes to this policy

Any modification will be published at this URL with an update date.
For substantial changes, we will display a notification in the App on
next launch.

## 15. Contact

Gaïalabx
Email: kiosqrssatm@gmail.com
App: Kiosq (com.gaialabx.kiosq)
