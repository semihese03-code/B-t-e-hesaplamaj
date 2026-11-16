# Bizim Bütçe

Bu depo, mevcut React tabanlı aile bütçe uygulamasını Vite + Capacitor 7 yapısıyla Android uygulama projesine dönüştürür.

## Gereksinimler

- Node.js 20+
- Java 21
- Android SDK

## Kurulum

```bash
npm install
npm run build
npx cap sync android
cd android
./gradlew assembleDebug
```

Debug APK dosyası:

```text
android/app/build/outputs/apk/debug/app-debug.apk
```

## GitHub Actions ile APK üretimi

`.github/workflows/android-debug-build.yml` dosyası otomatik olarak debug APK üretir ve GitHub Artifacts olarak yükler.
