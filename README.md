# PiratePrint Updates

This repository hosts the PiratePrint Android APK and update manifest.

Manifest URL:

```text
https://raw.githubusercontent.com/hexensohn/PiratePrint-Updates/refs/heads/main/pirateprint-update.json
```

APK URL:

```text
https://raw.githubusercontent.com/hexensohn/PiratePrint-Updates/refs/heads/main/PiratePrint.apk
```

## Publishing a new update

1. Increase `versionCode` and `versionName` in `app/build.gradle`.
2. Build the signed APK with `./gradlew.bat :app:assembleRelease`.
3. Replace `PiratePrint.apk` in this repository.
4. Update `pirateprint-update.json` so `versionCode`, `versionName`, and `apkUrl` match the new APK.

Android will require the APK to be signed with the same release key as the installed app.