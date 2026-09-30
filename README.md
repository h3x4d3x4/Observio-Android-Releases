# Observio for Android

Observio is a live TV and media player for Android phones and tablets, Android TV, Google TV and Fire TV, as well as Mac, iPhone and iPad. It plays your own IPTV playlists and provider logins (M3U, Xtream Codes, Stalker portals), Plex, Emby and Jellyfin libraries, and HDHomeRun tuners, with a full TV Guide, catch-up, movies and series. On a TV it switches to an interface built for the remote. Observio does not provide any channels or content; you bring your own sources.

This repository hosts the Android downloads (APK files) and the in-app update feed. The source code is private.

Website: [observio.hexadexa.io](https://observio.hexadexa.io)

## Download

Get the newest build from the [Releases page](https://github.com/h3x4d3x4/Observio-Android-Releases/releases). Each release contains:

- `Observio-Android-<version>.apk`: the app. One APK covers phones, tablets and TVs, on both 64-bit and 32-bit ARM devices.
- `SHA256.txt`: the checksum of the APK.

Builds are currently beta releases, marked *Pre-release* on GitHub.

**Phones and tablets:** download the APK on the device, open it and tap **Install**. The first time, Android asks you to allow installs from your browser or file manager.

**Android TV, Google TV and Fire TV:** follow the step-by-step guide at [observio.hexadexa.io/android](https://observio.hexadexa.io/android). Once installed, choose **Set up from phone** on the TV and scan the code with Observio on your phone to bring over your providers without typing on the remote.

## Requirements

- Android 8.0 or later
- Phones, tablets, Android TV, Google TV, Fire TV, streaming boxes and projectors

Observio is free to try. See [observio.hexadexa.io](https://observio.hexadexa.io) for details.

## Updates

Observio installed from this page keeps itself up to date:

1. About twice a day the app reads [`update.json`](update.json) from this repository.
2. When a newer build is listed, it shows the release notes and offers to install it.
3. Before installing, the app downloads the APK over HTTPS and checks its SHA-256 checksum against the one in `update.json`. Android then only accepts the update if it is signed with the same key as the installed app.

Beta builds follow the `beta` channel in `update.json`; release builds follow only the `stable` channel. You can turn automatic checks off, or check now, in the app's Settings. No other data is sent by the update check.

A future Google Play version will update through Google Play, never through this repository.

## Verifying downloads

Compare the APK's checksum with `SHA256.txt` from the same release, or with the `sha256` value in `update.json`:

```sh
shasum -a 256 Observio-Android-<version>.apk    # macOS / Linux
certutil -hashfile Observio-Android-<version>.apk SHA256    # Windows
```

## Release notes

- Each build's notes are on the [Releases page](https://github.com/h3x4d3x4/Observio-Android-Releases/releases).
- The full history across all platforms is at [observio.hexadexa.io/changelog](https://observio.hexadexa.io/changelog).

## Other platforms

- **Mac:** see [Observio for Mac](https://github.com/h3x4d3x4/Observio-Releases).
- **iPhone and iPad:** distributed through Apple. See [observio.hexadexa.io](https://observio.hexadexa.io) for availability.

## Support and privacy

- Help and FAQ: [observio.hexadexa.io/support](https://observio.hexadexa.io/support)
- Privacy policy: [observio.hexadexa.io/privacy](https://observio.hexadexa.io/privacy)
- Email [andrei@hexadexa.dev](mailto:andrei@hexadexa.dev). In the app, **Settings > Help** and **View Logs** help when reporting a problem.

---

Observio is made by [Hexadexa](https://hexadexa.io).
