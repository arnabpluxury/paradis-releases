```
 ===============================================================================
                                                                              
                         PPPPPP     AAAAA    RRRRRR     AAAAA     DDDDDD       
                         PP   PP   AA   AA   RR   RR   AA   AA    DD   DD      
                         PPPPPP    AAAAAAA   RRRRRR    AAAAAAA    DD   DD      
                         PP        AA   AA   RR  RR    AA   AA    DD   DD      
                         PP        AA   AA   RR   RR   AA   AA    DDDDDD       
                                                                              
 ===============================================================================
                                                                              
                    Premium Anime Streaming for Android                       
                    Official APK Releases & Public Documentation              
                                                                              
 ===============================================================================
```

```
  ..............................................  Status  .................................................
  Package .............. com.paradis.app
  Platform ............. Android (APK)
  Channel .............. Stable / Production
  Auth Provider ........ AniList OAuth2
  Source Code .......... Private (this repository distributes binaries only)
  ..............................................................................................
```

---

## Overview

**Paradis** is a production Android client for anime discovery, playback, and watch-list tracking.  
This repository is the **public release home** for signed APK builds, release notes, feature documentation, and support materials.

It is **not** the application source repository. Source code remains private.  
What you will find here:

| Asset | Purpose |
| --- | --- |
| Signed `.apk` builds | Installable production packages via [Releases](../../releases) |
| Feature documentation | Clear description of what the app does |
| Install & update guides | Safe side-load and in-app update instructions |
| Changelog | Version-by-version history |
| Support materials | Issue reporting and troubleshooting |

---

## Quick Start

```
  1. Open the latest GitHub Release
  2. Download the .apk asset (paradis.apk or paradis-vX.Y.Z.apk)
  3. On Android, allow installs from this source when prompted
  4. Install, launch Paradis, sign in with AniList
```

Full install guide: [`docs/INSTALL.md`](docs/INSTALL.md)

Latest package metadata (used by the in-app updater):

```
  ./version.json
```

---

## Feature Snapshot

```
  +-------------------------+-----------------------------------------------+
  | Area                    | Highlights                                    |
  +-------------------------+-----------------------------------------------+
  | Home Discovery          | Featured banners, rows, continue watching     |
  | Search & Browse         | Live metadata search + season aggregation     |
  | Playback                | Native player, gestures, quality / server     |
  | Audio                   | Sub / Dub switching with position preserved   |
  | Tracking                | AniList sync on progress milestones           |
  | Social                  | Threaded episode comments + like / dislike    |
  | Cast                    | Chromecast button (dev client builds)         |
  | Lists                   | My List / Browse synced with AniList           |
  | Updates                 | In-app APK update checks against this repo    |
  +-------------------------+-----------------------------------------------+
```

Full feature catalogue: [`docs/FEATURES.md`](docs/FEATURES.md)

---

## Releases

Production APKs are published on the GitHub **Releases** page only.

Expected asset naming:

```
  paradis.apk
  paradis-v1.1.0.apk   (optional versioned alias)
```

Release process for maintainers: [`docs/RELEASING.md`](docs/RELEASING.md)

```
  ..............................................  Update path  .............................................
  App boots
      |
      v
  Fetch /version.json from this repository (or backend mirror)
      |
      v
  Compare remote versionCode > installed nativeBuildVersion
      |
      v
  Prompt user -> download APK -> Android package installer (same applicationId)
  ..............................................................................................
```

---

## Documentation Index

| Document | Description |
| --- | --- |
| [`docs/FEATURES.md`](docs/FEATURES.md) | Complete product feature list |
| [`docs/INSTALL.md`](docs/INSTALL.md) | Install, permissions, troubleshooting |
| [`docs/RELEASING.md`](docs/RELEASING.md) | How maintainers publish APKs |
| [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md) | High-level product / system overview (no private source) |
| [`docs/FAQ.md`](docs/FAQ.md) | Common questions |
| [`CHANGELOG.md`](CHANGELOG.md) | Release history |
| [`SECURITY.md`](SECURITY.md) | Security & reporting |
| [`SUPPORT.md`](SUPPORT.md) | How to get help |
| [`LICENSE`](LICENSE) | Distribution terms |

---

## System Requirements

```
  . Android 8.0 (API 26) or newer recommended
  . Stable internet connection for catalog, streams, and AniList
  . Optional: Chromecast-compatible device for casting features
  . Optional: GitHub Releases access for first install / manual updates
```

---

## Screenshots & Brand

Place public marketing images under:

```
  ./assets/screenshots/
  ./assets/brand/
```

Do not commit private build secrets, keystores, or source archives to this repository.

---

## Roadmap Signals

```
  [x] AniList authentication & list sync
  [x] Native player (no WebView playback)
  [x] Sub / Dub source separation
  [x] Continue Watching timestamps
  [x] Threaded comments
  [x] In-app version updater pipeline
  [ ] Broader cast-device QA matrix
  [ ] Expanded browse taxonomies
```

Product status notes may change as release cadences continue. Details stay in [`CHANGELOG.md`](CHANGELOG.md).

---

## Disclaimer

```
  ..............................................................................
  . Paradis aggregates publicly reachable catalog metadata and streams from    .
  . third-party sources at the user's device. Availability of any title,        .
  . server, subtitle track, or cast path depends on upstream providers and      .
  . network conditions. Use of the app must comply with your local laws and     .
  . the terms of connected services (including AniList).                        .
  ..............................................................................
```

---

## Maintainers

```
  Project ............... Paradis
  Public package id ..... com.paradis.app
  Release channel ....... GitHub Releases (this repository)
```

For security reports, follow [`SECURITY.md`](SECURITY.md).  
For user support, start with [`SUPPORT.md`](SUPPORT.md).

```
 ===============================================================================
                         end of README  ::  Paradis public release hub
 ===============================================================================
```
