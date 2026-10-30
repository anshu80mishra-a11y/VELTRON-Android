# VELTRON Technologies — Android APK project

This packages the current VELTRON website inside an Android WebView app. The main page is
bundled in the APK and can open offline. External links and email actions need internet or
a compatible app.

## Build with GitHub Actions
1. Create a GitHub repository named `VELTRON-Android`.
2. Upload the **contents** of this project folder to the repository root. The `app/`,
   `.github/`, `build.gradle`, and `settings.gradle` entries must be at the top level.
3. Open **Actions** → **Build VELTRON APK** → **Run workflow**.
4. Wait for the run to finish successfully.
5. Open the run and download the `VELTRON-Android-APK` artifact.
6. Extract the downloaded ZIP; it contains `app-debug.apk`.

A push to the `main` branch also triggers a build.

## Important
- This is build-ready source; a compiled APK is not included yet.
- Treat it as build-verified only after GitHub Actions succeeds.
- This is a debug/testing APK, not a Play Store release.
- Never commit signing keys, passwords, API keys, or OTPs.
- The website contact form opens the device email app; it does not store or send messages itself.
