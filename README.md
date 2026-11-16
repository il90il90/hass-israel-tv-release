# Israel TV — releases

Downloads of the **Israel TV** app for Android TV, Google TV and Android phones: Israeli live TV channels, built for the remote control on a television and for touch on a phone. The app needs an Israel TV license.

**[Download the latest APK](https://github.com/il90il90/hass-israel-tv-release/releases/latest/download/israel-tv-tv.apk)** · [All versions](https://github.com/il90il90/hass-israel-tv-release/releases)

On a TV, install it with a file manager or over adb:

```
adb install israel-tv-tv.apk
```

On a phone, the easiest way to install it and keep it up to date is [Israel App Manager](https://github.com/il90il90/israel-app-manager), which lists all of my apps.

## How a release gets here

The source code lives in a private repository. A signed APK is pushed to the `release-inbox` branch together with a `release.json`; the *Publish release* workflow checks that it is signed with the key whose fingerprint is in [`signing-cert.sha256`](signing-cert.sha256) and turns it into a tagged release. The link above always points at the newest one.
