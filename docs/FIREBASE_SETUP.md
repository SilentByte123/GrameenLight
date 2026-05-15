# Firebase Setup

## Purpose

Firebase Firestore is used as the remote sync layer for Grameen-Light. The application still works locally without Firebase because Room Database is used for offline-first storage.

## Current Repository Setup

This repository includes the Android Firebase configuration file used for the demo build:

- `app/google-services.json`

With the current Firebase project and rules, a fresh clone should be able to build and use Firestore sync directly.

## Important Notes

- The app still supports Room-only local storage if Firebase becomes unavailable
- Sync states such as `Pending`, `Synced`, and `Failed` depend on actual Firebase availability
