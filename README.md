# LEA Timber Shade Masjid — Building Fund Tracker

Mobile-first tracker for the masjid fundraising target of ₦1,000,000.

## Setup required before launch
1. Register a Firebase Web app and put its client configuration in `firebase-config.js`.
2. Enable Email/Password under Firebase Authentication.
3. Create the authorized administrator in Authentication and copy their UID.
4. Replace `PASTE_ADMIN_AUTH_UID_HERE` in both `firebase-config.js` and `firestore.rules`.
5. Create Firestore Database and publish `firestore.rules`.
6. Deploy using GitHub Pages. In Settings > Pages, choose GitHub Actions, then check the Actions tab for the deployment URL.

Only the configured administrator UID can change donation records according to Firestore Rules. Public read access means donor names and amounts are visible to visitors; get committee approval before publishing. Never commit passwords or service-account private keys.

The 13 starter records from the previous preview (₦65,000 total) are not automatically migrated to Firestore. Verify and enter them deliberately to avoid duplicates.

## Final tests
- [ ] Live updates work across two devices.
- [ ] Admin can add, edit, delete, and export.
- [ ] Anonymous and non-admin users cannot write.
- [ ] WhatsApp sharing and group invite work.
- [ ] Verify account details with the committee before launch.


Deployment status check requested on 2026-10-09.
