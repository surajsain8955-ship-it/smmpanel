# IncreserMaster — GitHub Actions APK Build

This project now includes a GitHub Actions workflow that builds a downloadable
Android debug APK in GitHub's cloud runner. GitHub Actions can build artifacts
on GitHub-hosted runners, so Android Studio is not required on your Mac.

## 1. Create a GitHub repository

Create a new repository on GitHub, for example:

`incresermaster-android`

A public repository is the simplest route for this project.

## 2. Upload this project

Extract this ZIP, then upload the project files/folders to the repository.

Make sure these are at the repository root:

- `app/`
- `build.gradle.kts`
- `settings.gradle.kts`
- `gradle.properties`
- `.github/workflows/build-apk.yml`

Do NOT upload the outer ZIP file as the only repository file.

## 3. Start the build

After uploading, open the repository on GitHub and:

**Actions → Build IncreserMaster APK → Run workflow**

The workflow also runs automatically when you push to `main` or `master`.

## 4. Download the APK

Wait for the workflow to finish with a green check.

Open the completed workflow run and scroll to **Artifacts**.

Download:

`IncreserMaster-debug-apk`

Inside it is:

`app-debug.apk`

Copy that APK to your Android phone and install it.

## Notes

- This is a debug APK intended for testing/direct installation.
- It does not require an Emergent subscription.
- It does not require Android Studio on your Mac.
- The app loads `https://incresermaster.com/` in a native Android WebView.
- For Google Play publishing, a properly signed release/AAB build is required.
