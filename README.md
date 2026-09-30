# IncreserMaster Android WebView App

This project is a simple native Android application that opens:

https://incresermaster.com/

inside an Android WebView.

## Build a debug APK

1. Install Android Studio.
2. Open this folder as an existing project.
3. Let Gradle sync/download the Android Gradle Plugin.
4. Select **Build > Build App Bundle(s) / APK(s) > Build APK(s)**.
5. The debug APK will normally be in:
   `app/build/outputs/apk/debug/app-debug.apk`

## Build a release APK

Use Android Studio:
**Build > Generate Signed App Bundle / APK > APK**

For Google Play, use an **Android App Bundle (.aab)** rather than an APK.

## What is included

- IncreserMaster app name
- Website loaded automatically in WebView
- JavaScript and DOM storage
- Login/session cookies
- Android back-button navigation
- File upload support
- Download support
- External handling for non-http(s) links
- Portrait orientation
- Loading indicator

## Important

This is an Android application project, not a forced PWA. The website remains hosted at incresermaster.com. Changes to the website can therefore appear in the app without rebuilding the app.

You still need Android Studio/Android SDK to compile the APK. No Emergent subscription is required for this project.


## GitHub Actions

This project includes `.github/workflows/build-apk.yml`. Upload the project to GitHub, then use **Actions → Build IncreserMaster APK → Run workflow**. The completed run provides `IncreserMaster-debug-apk` as a downloadable artifact.
