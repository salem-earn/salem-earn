# 🔥 Salem Earn - Android Studio & APK Build Package
Package: com.salem.earn
Google Mobile Ads App ID: ca-app-pub-7078246007336691~3232855268
Banner Ad Unit ID: ca-app-pub-7078246007336691/9754865735
Rewarded Ad Unit ID: ca-app-pub-7078246007336691/1969901177

## Prerequisites
1. Android Studio (Hedgehog or newer) with Android SDK 34
2. Java JDK 17 or JDK 21
3. Node.js 18+

## Quick Build Steps to generate APK:
1. In your root web project, build the production web bundle:
   npm run build
2. Sync assets to the Android project:
   npx cap sync android
3. Generate the Debug APK:
   cd android
   ./gradlew assembleDebug
   (Or in Windows: gradlew.bat assembleDebug)

The generated APK will be located at:
android/app/build/outputs/apk/debug/app-debug.apk

## Generate Release APK for Play Store:
   cd android
   ./gradlew assembleRelease
