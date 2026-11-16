# Israel TV — releases

Downloads of the **Israel TV** app for Android TV, Google TV and Android phones: Israeli live TV channels, built for the remote control on a television and for touch on a phone. The app needs an Israel TV license.

**[Download the latest APK](https://github.com/il90il90/hass-israel-tv-release/releases/latest/download/israel-tv-tv.apk)** · [All versions](https://github.com/il90il90/hass-israel-tv-release/releases)

On a TV, install it with a file manager or over adb:

```
adb install israel-tv-tv.apk
```

On a phone, the easiest way to install it and keep it up to date is [Israel App Manager](https://github.com/il90il90/israel-app-manager), which lists all of my apps.

## How a release gets here

The source code lives in a private repository. After each release there, its *Public release* workflow checks that the APK is signed with the key whose fingerprint is in [`signing-cert.sha256`](signing-cert.sha256) and copies it here, so the links above always point at the newest one.

A release can also be handed in by pushing a signed APK and a `release.json` to the `release-inbox` branch; the *Publish release* workflow here makes the same check and creates the release.
