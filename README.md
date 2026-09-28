# KalingApp — Mobile App Downloads

Debug builds of the KalingApp mobile application, published here so they can be
installed on a phone without needing access to the source repository.

## Download

**[kalingapp-v1.0-debug.apk](kalingapp-v1.0-debug.apk)** — 20.4 MiB

Updated 2026-09-29: fixes the Forgot Password screen showing "Resetting…"
before you'd touched it, and "Sending…" stuck after tapping back. Same
signing certificate as the previous build, so installing over it works
without uninstalling first.

On a phone, tap the link above, then tap **Download**. Open the file when it
finishes and Android will ask to install it.

## Installing

This is a debug build signed with Android's standard debug certificate, not a
Play Store release, so Android will warn you before installing it. That warning
is expected.

1. Download the APK using the link above.
2. Open it. Android will say installs from this source are blocked.
3. Tap **Settings**, turn on **Allow from this source**, then go back.
4. Tap **Install**.

If you previously installed a build signed with a different key, uninstall the
old copy first — Android refuses to replace an app when the signing certificate
does not match.

## This build

| | |
|---|---|
| Version | 1.0 (versionCode 1) |
| Package | `com.aistudio.kalingapp.hsmqwr` |
| Requires | Android 7.0 (API 24) or newer |
| Built against | Android API 36 |
| Size | 21,402,825 bytes |
| SHA-256 | `a7f96f7aa0c4aecebb113d658db48f58413b1cc1013cd7c4ad15b88662db9599` |
| Signing | Debug certificate, V2 scheme (SHA-256 `a2b8…3b5e`) |
| Source commit | `KalingApp-Prototype@1423e83` |

To confirm the file downloaded intact, compare the SHA-256:

```bash
sha256sum kalingapp-v1.0-debug.apk        # Linux / macOS / Git Bash
certutil -hashfile kalingapp-v1.0-debug.apk SHA256   # Windows
```

## Notes

Milk volumes throughout the app are millilitres. The admin console displays
facility stock in litres, but that is display formatting over the same stored
millilitres — there is no second unit anywhere in the system.

The app talks to the live backend on Render, which sleeps after 15 minutes of
inactivity on the free plan. The first request after a quiet period can take
10–30 seconds while the server wakes up. That is expected, not a failure.

This repository holds built artifacts only. The application source lives in a
separate, private repository.
