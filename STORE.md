# Store Preparation Checklist

## PWA (web install)
Already works on iOS Safari "Add to Home Screen" and Android Chrome "Install app".

## iOS App Store
1. Join Apple Developer Program ($99/year)
2. Use Tauri to build `src-tauri/target/release/bundle/macos/*.app`
3. Sign with Apple Developer ID / Distribution certificate
4. Upload via Transporter or Xcode
5. Provide screenshots (6.5", 5.5", iPad), privacy policy URL, app description

## Google Play Store
1. Create Google Play Developer account ($25 one-time)
2. Build Android APK/AAB — Tauri supports this via `cargo tauri android build`
3. Sign with upload key
4. Upload AAB to Play Console
5. Provide screenshots (phone + tablet), privacy policy, content rating

## macOS / Windows direct distribution
GitHub Actions builds MSI (Windows), DMG (macOS), AppImage/deb (Linux). Download from GitHub Releases.
