# PixCut Update Server

This repository hosts the free update server for PixCut app using GitHub Pages.

## Files

- `update.json` - Contains version information and update details
- `latest.apk` - The latest PixCut APK build (you need to upload this)

## URLs

- Update Info: https://katsuki-445.github.io/pixcut-updates/update.json
- APK Download: https://katsuki-445.github.io/pixcut-updates/latest.apk

## How to Update

1. Build new APK from Android Studio
2. Replace `latest.apk` with new build
3. Update `update.json`:
   - Increment `versionCode`
   - Update `versionName`
   - Add new changelog entries
4. Commit and push changes
5. All users get automatic updates!

## Version Format

- `versionCode`: Must be higher than current app version
- `versionName`: User-friendly version string
- `forceUpdate`: Set to true for critical updates
- `minSupportedVersion`: Minimum version that can still run the app
