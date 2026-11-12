# BitAim v2.0

Android screen-overlay aim-line assistant for Carrom-style games. This customized build is line-only: it does not automate taps, swipes, or shots.

**Line-only build**
- Auto-detection of striker, coins and pockets via OpenCV + screen capture
- Multi-line trajectory prediction (direct, coin chains, 1- and 2-cushion bounces)
- AutoPlay (removed in this line-only build) and accessibility gesture injection removed from the app interface and manifest
- Pocket-prediction highlight

See `HOW_TO_BUILD.md` for full build instructions.

This is **source code only** — you must build the APK yourself in Android Studio.

## Permissions
- "Display over other apps" (one-time)
- Screen capture / MediaProjection (per-session — Android requires this every time)
- POST_NOTIFICATIONS on Android 13+

## Quick start (two ways)

### Easiest: let GitHub build the APK for you
See **`GITHUB_BUILD_GUIDE.md`** — no PC tools needed, just a free GitHub account.
The repo includes a `.github/workflows/build-debug-apk.yml` that compiles the debug APK
automatically and lets you download it from the Actions tab.

### Or build locally on your PC
```bash
npm install
# then open android/ in Android Studio and Build > Build APK(s)
```
See `HOW_TO_BUILD.md` for the full local-build instructions.
