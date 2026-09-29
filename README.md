# Observio for Android

**A modern IPTV player for Android phones, tablets, Android TV, Google TV, Fire TV, boxes and projectors.** Live TV, movies and series, a full programme guide and catch-up, in one app. Bring your own provider; Observio is the player.

This repository holds the public Android downloads (APK files) and the automatic-update feed. The source code is private.

## Download

Get the newest build from the [**Releases**](../../releases) page. Test builds are marked *Pre-release*.

- **Phones and tablets:** download `Observio-Android-<version>.apk` on the device, open it and tap **Install**. If Android asks, allow installs from your browser or file manager once.
- **Android TV, Google TV, Fire TV, boxes and projectors:**
  - With the **Downloader** app, enter the APK's link from the Releases page.
  - Or from a computer: `adb connect <tv-ip>:5555`, then `adb install Observio-Android-<version>.apk`.
  - On TV devices Observio opens in its TV interface automatically. Settings › Interface can switch it.
- Needs **Android 8.0** or newer. One APK covers 64-bit and 32-bit ARM devices.
- Each release also has a `SHA256.txt` so you can check the download.

> The Google Play version, when it ships, updates through Google Play and never through this page.

## What Observio does

- **Live TV** with groups, favourites, a live preview, fast channel changes, and number and CH ± keys on remotes that have them.
- **Programme guide** where every programme can be selected, with catch-up and reminders.
- **Movies and series** from your provider, with artwork and resume.
- **Two playback engines**, chosen per channel, so broadcast FHD channels that phone decoders can't start still play.
- **Pause Live TV**, recording (sideload builds), Chromecast, subtitles.
- **On TVs:** switches to 50 Hz for European channels and 24 Hz for films, sends surround sound to your receiver, and lets you **set it up from your phone**: scan the code on the TV and your providers, guides, favourites and licence arrive without typing.
- Works with **Xtream Codes** and **M3U** playlists.

Observio does not provide any channels, streams or content. You supply your own provider or playlist.

## Licence

The same on every device: **30 days with everything unlocked**, then **Observio Free** keeps working (live TV, the full guide, your provider's movies and series). A **one-time purchase** unlocks the rest for good: more providers, catch-up, multi-view, reminders and more. A licence sent from your phone with *Set up from phone* unlocks your TV as well.

## Automatic updates

Sideloaded builds keep themselves up to date. Twice a day Observio reads [`update.json`](update.json) from this repository. When a newer build is out it shows what's new and installs it with one tap. Android only accepts an update signed with the same key as the installed app. You can turn the checks off, or check any time, in **Settings › Updates** (on TV: **Settings › This Device**). Nothing else is sent.

Test builds (*Pre-release*) follow the beta channel. Release builds only get releases.

## Support

Email **andrei@hexadexa.dev**. In the app, **Settings › Help** and **View Logs** help with bug reports.
