# Delete your Pocketa account and data

**Applies to:** Pocketa (`com.yashtries.voicebudget`) for Android
**Effective date:** 6 November 2026

Pocketa works without an account. If you enabled the optional Firebase cloud
backup, an account exists under your Google sign-in. This page explains how to
delete your data and what is deleted or kept.

## Delete local data on your device

1. Open Pocketa.
2. Go to **Settings**.
3. Tap **Delete all data** and confirm.

Uninstalling the app also removes all local data. This does **not** delete a
Firebase cloud backup.

## Delete your cloud backup and account

1. Email **Sareenash94@gmail.com** from the Google account you used for backup.
2. Use the subject **"Delete my Pocketa data"**.
3. We will verify ownership of the account and delete the Cloud Firestore
   records stored under your user ID, then confirm by email.

Turning off Firebase cloud backup in Settings stops future syncing, but it does
not delete data that is already stored in the cloud. Follow the steps above to
delete existing cloud data.

## What is deleted

- **Local data:** expenses, categories and settings. Deleted immediately when
  you use **Delete all data** or uninstall the app.
- **Cloud backup data:** categories and expenses stored in Cloud Firestore under
  your Firebase user ID. Deleted within 30 days of a verified request.

## What is kept

- **Hashed installation identifiers and quota counters:** retained only as long
  as needed to enforce usage limits. They are not linked to your name, email or
  Google account.
- **Crashlytics crash reports:** retained by Google according to its retention
  schedule. They contain technical crash information only, not expense content,
  transcripts or voice recordings, and are not linked to your account.
- **Aggregated, non-identifying usage totals:** used only to operate and monitor
  the service and are not linked to your account.

## Retention periods

- Local data: deleted immediately.
- Cloud backup data: deleted within 30 days of a verified request.
- Hashed quota counters: retained only as long as needed to enforce usage
  limits.

## Contact

For deletion requests or questions: **Sareenash94@gmail.com**

See also: [Pocketa Privacy Policy](https://yashtries.github.io/pocketa-privacy/)
