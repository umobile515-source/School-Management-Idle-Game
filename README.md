# School Tycoon Idle - Android (Capacitor)

The game is a web app (`www/index.html`, Three.js) wrapped as an Android app.

## Option A: build on your computer
Install Node 18+, Android Studio (or JDK 17 + Android SDK), then:

    npm run setup      # installs packages, bundles Three.js offline, creates android/
    npm run apk        # builds android/app/build/outputs/apk/debug/app-debug.apk

Or run `npm run open` to open the project in Android Studio and press Run on your phone.

## Option B: build in the cloud (no Android tools needed)
1. Create a free GitHub repository and upload this whole folder.
2. Open the Actions tab -> "Build Android APK" -> Run workflow.
3. Download `school-tycoon-debug-apk` from the finished run and install the APK
   on your phone (allow "install unknown apps").

## Notes
- After editing `www/index.html`, run `npm run sync` and rebuild.
- A debug APK is fine for testing. For Google Play you need a signed release
  build (Android Studio: Build > Generate Signed Bundle).
