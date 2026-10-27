# BetterOSD

Bring back the classic volume and brightness feedback overlay to the center of your screen on macOS.

![BetterOSD screenshot](screenshot.png)

## Download
1. Download the latest **BetterOSD-arm64.dmg**: [Download](https://github.com/zmlabs/better-osd/releases/latest/download/BetterOSD-arm64.dmg)
2. Open the DMG and drag **BetterOSD.app** into **Applications**.
3. Launch the app.

## Build artifacts

The **Build macOS App** GitHub Actions workflow compiles the app on branch pushes and pull requests. Open a successful run in the repository's **Actions** tab and download the **BetterOSD-arm64** artifact, which contains a DMG installer and a ZIP of the app. Artifacts are kept for 14 days, and build logs are uploaded separately.

These Apple Silicon builds use ad hoc signing and do not require Apple Developer secrets. They are not notarized, so macOS may require you to allow the app in **System Settings → Privacy & Security**. The existing **Release (Notarized DMG)** workflow still requires signing and notarization secrets.

Once the build workflow is on the default branch, you can also start it manually with **Run workflow**.

## App Store
**App Store link:** https://apps.apple.com/us/app/volume-hud/id6752903119  
Due to the use of private APIs and Accessibility permissions, we can no longer ship updates via the App Store. The App Store version will not be updated.

## Notes
- You'll be prompted for **Accessibility** permission so BetterOSD can listen to media keys.
- Supports both volume and brightness HUD feedback.
- Only supports Apple Silicon (M-series Macs).
