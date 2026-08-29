# Sean's Sec Lab — Native App

App ID: `com.seanfrvr.seclab`

## Android

Requires Node 22+, JDK 21, and Android SDK.

```bash
npm install
npx cap add android
npx cap sync android
cd android
./gradlew assembleDebug
```

Debug APK output:
`android/app/build/outputs/apk/debug/app-debug.apk`

## iPhone / iPad

Capacitor 8 targets modern iOS. A Mac with current Xcode and Apple signing is required for distribution.

```bash
npm install
npx cap add ios
npx cap sync ios
npx cap open ios
```

Then select your Apple Developer team in Xcode and distribute through TestFlight/App Store.

## Web

The `www/` folder remains the shared offline-first study app source.
