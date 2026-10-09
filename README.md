# Zoro Media Manager

Android source project for the Zoro Media Manager app.

## Build APK on GitHub (phone-friendly)

1. Create a new GitHub repository and upload the **contents** of this folder to its root (so `.github/workflows/android-build.yml` is at the repository root and `settings.gradle` is in `ZoroMediaManager/`).
2. In GitHub, open **Actions** and select **Build Android APK**.
3. Tap **Run workflow**. The workflow installs Java, Android SDK components, and Gradle, then runs `assembleDebug`.
4. When the run succeeds, open the run page and download **ZoroMediaManager-debug-apk** under Artifacts.

The workflow builds a debug APK. This environment has no Android SDK installed and cannot reach external package repositories, so the APK has not been compiled or device-tested here. The first GitHub build may take several minutes while dependencies are downloaded.

## Features

- Shared profile image bundled as `app/src/main/assets/zoro.jpg`.
- Pick post images from the device.
- Manage account labels locally in the app.
- Manual workflow checklist and option to open an installed Honista app.
- No Instagram password/2FA storage and no automated login or posting.
