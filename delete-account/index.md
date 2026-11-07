# Delete your Pocketa data or account

**Applies to:** Pocketa (`com.yashtries.voicebudget`) for Android
**Effective date:** 6 November 2026

Pocketa works without an account. If you enabled the optional Firebase cloud
backup, an account exists under your Google sign-in. You can delete some or all
of your data without deleting your account, or ask us to delete the account as
well. This page explains how, and what is deleted or kept.

## Delete local data on your device

1. Open Pocketa.
2. Go to **Settings**.
3. Tap **Delete all data** and confirm.

Uninstalling the app also removes all local data. This does **not** delete a
Firebase cloud backup.

## Delete cloud data without deleting your account

1. Email **Sareenash94@gmail.com** from the Google account you used for backup.
2. Use the subject **"Delete my Pocketa data"**.
3. We will verify ownership of the account and delete the Cloud Firestore
   records stored under your user ID, then confirm by email. Your Google and
   Firebase sign-in account remains active, but it will have no Pocketa backup
   data.

Turning off Firebase cloud backup in Settings stops future syncing, but it does
not delete data that is already stored in the cloud. Follow the steps above to
delete existing cloud data.

## Delete your account as well

1. Email **Sareenash94@gmail.com** from the Google account you used for backup.
2. Use the subject **"Delete my Pocketa account"**.
3. We will verify ownership, delete the Cloud Firestore records under your user
   ID and delete the Firebase Authentication user, then confirm by email.
4. Delete the app's local data separately (Settings → **Delete all data**, or
   uninstall the app).

## What is deleted

- **Local data:** expenses, categories and settings. Deleted immediately when
  you use **Delete all data** or uninstall the app.
- **Cloud backup data:** categories and expenses stored in Cloud Firestore under
  your Firebase user ID. Deleted within 30 days of a verified request.
- **Account (only if requested):** the Firebase Authentication user associated
  with your Google sign-in. Deleted within 30 days of a verified request.

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
