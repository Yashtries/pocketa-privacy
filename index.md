# Pocketa Privacy Policy

**Effective date:** 6 November 2026
**Applies to:** Pocketa (`com.yashtries.voicebudget`) for Android
**Published at:** https://yashtries.github.io/pocketa-privacy/

Pocketa is a voice-first expense tracker. This policy explains what data the
app handles, why it is handled, and the choices you have. It applies to the
Pocketa Android app and the voice parsing service it uses.

## Summary

- Expenses, categories and settings are stored on your device by default.
- Voice recordings are sent to our parsing service and forwarded to Google's
  Gemini API to turn speech into expense details. Audio is not stored.
- Google sign-in and cloud backup are optional.
- Crash reports are sent only when the app crashes.
- No advertising, no analytics, no tracking, and no selling of personal data.

## Voice entry and AI processing

- When you record an expense, the audio file is sent over HTTPS to our
  Cloudflare Worker endpoint (`/v1/parse-expense`) and forwarded to Google
  Gemini for transcription and parsing.
- The Worker does not store audio files or transcripts.
- A random installation identifier is hashed with SHA-256 and stored together
  with usage counters in Cloudflare D1 so that per-install usage limits can be
  enforced. The identifier is not linked to your name, email or Google account.
- The parsed expense (amount, category, date, note and the original transcript)
  is returned to the app and saved in the on-device database.
- Voice recordings are not used for model training and are not retained by the
  parsing service.

## Local storage

- Expenses, categories and settings live in an on-device database.
- Local JSON backup files created with export/import are not encrypted, so
  store them somewhere you trust.

## Optional cloud backup (Firebase)

- Google sign-in is optional and uses Firebase Authentication. Signing in is
  only required if you choose to use cloud backup.
- If enabled, categories and expenses may be stored in Cloud Firestore under
  your account's user ID. Security rules restrict access to the owning account.
- Data is protected in transit by Firebase, but is stored unencrypted at the
  application layer.
- Disabling or deleting your backup does not delete the app's local data, and
  deleting the app does not delete cloud backup data.

## Crash reports

- Release builds use Firebase Crashlytics. If the app crashes, a report is sent
  that contains the crash stack trace, app version, device model, operating
  system version, and technical state at the time of the crash.
- Crash reports do not include your expense content, transcripts, or voice
  recordings.
- Crashlytics does not receive advertising identifiers. Reports are used only to
  diagnose and fix defects, and are processed by Google as our service
  provider.

## Data the app handles and permissions

- The app requests only the `INTERNET` and `RECORD_AUDIO` permissions.
- It does not collect contacts, location, photos, calendars, analytics or
  advertising identifiers.
- User-entered expense content (amount, category, date, note, currency, payment
  method and transcript) is the only personal content the app stores.

## Third parties

- **Cloudflare** (Workers, D1, Access): hosts the parsing service, enforces rate
  limits and protects the owner dashboard.
- **Google** (Firebase Authentication, Cloud Firestore, Crashlytics, Gemini):
  sign-in, optional cloud backup, crash reports and AI expense parsing.

Each provider processes data only as needed to operate the service described
above.

## Retention and deletion

- Local data can be exported, edited or deleted in the app, and is removed when
  you uninstall the app.
- Cloud backup data remains in your Firebase project until it is deleted. To
  request deletion of cloud backup data, contact us at the address below; we
  will delete records associated with your account.
- Usage counters stored as hashed installation identifiers are retained only as
  long as needed to enforce usage limits.

## Security

- Network traffic between the app and our services uses HTTPS.
- No method of transmission or storage is completely secure, but we limit the
  data we keep and do not store voice recordings.

## Children

- Pocketa is not directed at children under the applicable age of digital
  consent, and we do not knowingly collect data from them.

## Changes

- Policy changes are published at this URL with an updated effective date.

## Contact

- Support and privacy requests: Sareenash94@gmail.com
