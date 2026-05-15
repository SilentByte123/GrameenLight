# Firebase Setup

## Purpose

Firebase Firestore is used as the remote sync layer for Grameen-Light. The application still works locally without Firebase because Room Database is used for offline-first storage.

## Required Steps

1. Create a Firebase project
2. Add an Android app with package name:

   `com.grameenlight.app`

3. Download `google-services.json`
4. Place the file in:

   `app/google-services.json`

5. Enable Firestore Database
6. Configure valid Firestore rules
7. Rebuild the Android project

## Important Notes

- `google-services.json` is not committed to GitHub
- Without Firebase configuration, the app continues to work with Room-only local storage
- Sync states such as `Pending`, `Synced`, and `Failed` depend on actual Firebase availability
