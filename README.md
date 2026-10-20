# Learn Cards: build the signed APK in the cloud

1. Create a **private** GitHub repository and upload everything in this folder (including `.github`).
2. Repo > Settings > Secrets and variables > Actions > New repository secret
   Name: `KEYSTORE_PASSWORD`   Value: the password you were given.
3. Actions tab > "Build APK" > Run workflow (or just push a change).
4. Download **LearnCards-signed-apk** (install on phone) or **LearnCards-play-store-aab** (upload to Google Play).

IMPORTANT: `android/app/release.keystore` is your app's identity. Back it up (and its password) somewhere safe.
If you lose it you can never update the app under the same signature. Keep the repo private.

To change the app: edit `www/index.html`. Raise `versionCode` in `android/app/build.gradle` before each new Play Store upload.
