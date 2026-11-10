# Redline Eats Delivery Calculator - Android

A standalone Android WebView wrapper for the offline Redline Eats delivery calculator.

## Build without installing Android Studio (GitHub)
1. Create a private GitHub repository.
2. Upload the contents of this folder, preserving `.github/workflows/build-apk.yml`.
3. Open the repository's **Actions** tab and select **Build installable Android APK** -> **Run workflow** (or push to main).
4. After a successful build, download the **Redline-Eats-Calculator-APK** artifact and extract it.
5. Transfer `app-debug.apk` to your Android phone/tablet and open it to install. Android may require allowing installs from this source.

This is a debug-signed APK for private internal use, not a production Play Store release. Do not upload a debug-signed APK to the Play Store. APK compilation and device installation have not been verified in this environment.

## Alternative: Android Studio
Open this directory as a project. Let Gradle sync, then choose Build > Build APK(s). Java 17 and Android SDK 35 are required.

## Behavior
- Calculator runs offline and stores settings in local WebView storage.
- Google Maps directions opens in the browser/Maps app and requires internet.
- Staff must manually enter road distance.
- Enter verified MPG and gasoline price before quoting.
- No customer orders are transmitted.
