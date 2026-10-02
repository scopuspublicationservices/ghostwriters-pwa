# Ghostwriters Android App

Android WebView application for https://www.ghostwriters.co.in/

- App name: Ghostwriters
- Package/Application ID: `ghostwriting.ghostwriters`
- Version: 1.0 (versionCode 1)
- Orientation: portrait
- Minimum Android: API 23
- Target Android: API 35

## What is included

- Android Studio project
- Ghostwriters logo/app icon
- WebView loading `https://www.ghostwriters.co.in/`
- JavaScript and DOM storage support
- Android file-picker support for website upload forms
- Android back-button navigation
- External handling for phone, email, WhatsApp and non-Ghostwriters web links
- GitHub Actions workflow for building a debug APK and an unsigned release AAB

## Build locally

Open this folder in Android Studio. Let Gradle sync, then use:

**Build > Build Bundle(s) / APK(s) > Build APK(s)**

For Google Play:

**Build > Generate Signed Bundle / APK > Android App Bundle**

Create and securely retain the release/upload keystore. Do not commit the keystore or passwords to GitHub.

## Important

The GitHub Actions workflow produces an **unsigned** release AAB. Google Play requires the release/upload artifact to be signed. Use Android Studio's signing flow or configure GitHub Actions secrets for a secure signing setup.
