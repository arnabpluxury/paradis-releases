```
 ===============================================================================
  PARADIS  ::  CHANGELOG
 ===============================================================================
```

All notable public releases are documented in this file.  
Versioning follows SemVer for `latestVersion` and a monotonic integer for `versionCode`.

---

## [Unreleased]

```
  . (none)
```

---

## [2.0.26] - 2026-10-28

```
  versionCode ...... 226
  buildHash ........ d207dd7bdef9
  size ............. ~79.8 MB
  sha256 ........... 72ed67729a16bb0a1979e067836ccf9e2e924297c5983eee9ce012e9cf60b37f

  Added
  ..... Live SUB | DUB badges from source catalog pages
  ..... Realtime episode comments with votes + emoji reactions (fire / love / laugh / sad / wow)
  ..... Title page Community thread (series-wide) separate from per-episode player talk
  ..... Daily trending push + in-app event from AniList charts
  ..... Stream catalog fallbacks (aniwaves.ru and additional mirrors); device still plays media
  ..... Profile username, accent color, longer bio, social link normalization

  Changed
  ....... Season picker episode counts come from scraper lists — no mock/estimated 12-ep fills
  ....... Bottom sheets and press animations tuned for smoother motion; less frosted glass on badges
  ....... Adaptive text scaling capped to reduce oversized-font layout glitches
  ....... API host: https://api.synerstudio.net.in (metadata/scraper only — no video proxy)
  ....... Chromecast play-services pinned to 21.5.0 / MediaRouter 1.8.1 for compileSdk 36
  ....... Event + update popups only after sign-in (never on login/register)

  Fixed
  ..... Episode like counts persist correctly to the database
  ..... Comment likes no longer stay as local-only state
  ..... EAS Android cloud build path issues (Windows autolinking cache + Cast dependency clash)
  ..... Trending event modal taps (close / CTA) frozen inside Android Modal
  ..... Green same-version patch dialog looping after Later / while already current
```

---

## [2.0.25] - 2026-07-29

```
  versionCode ...... 225
  buildHash ........ b4e8f21c9d03

  Fixed
  ..... Chromecast — location permissions + in-app device scanner
  ..... Browse & My Lists — black void under tabs
  ..... Anime details — cache + long-series episode counts
  ..... Manga reader — progress bar, retry, chapters list
  ..... Player sheets over video; Continue Watching realtime updates
```

---

## [2.0.21] - 2026-07-20

```
  versionCode ...... 221
  buildHash ........ cb32c1498f76

  Added
  ..... Smart OTA — buildHash detection for same-version bug-fix APK re-uploads
  ..... Patch vs version update modal (BUG FIX UPDATE / NEW VERSION)

  Changed
  ....... version.json schema: buildHash, forceUpdate, size, checksum, releaseNotes[]
  ....... Updater skips auto-prompt in __DEV__; re-checks every 30 minutes

  Notes
  ..... To ship a same-version fix: re-upload APK, run node scripts/new-build-hash.js,
        update buildHash in all version.json copies, deploy
```

---

## [2.0.20] - 2026-07-20

```
  versionCode ...... 220

  Added
  ..... Manga mode powered by MangaDex — home feed, genres, search, personal library
  ..... Manga reader with horizontal page & vertical scroll modes
  ..... HD / data-saver image quality, offline page cache, chapter picker, reading progress (expo-sqlite)
  ..... Anime ↔ Manga toggle in app header; dedicated manga bottom tab bar
  ..... Chapter-update checks in foreground (production builds)

  Changed
  ....... Streaming UI polish — #E03C3C accent, Bebas/Outfit/Space Grotesk typography, glass surfaces
  ....... Cast icon centered under notch; sharp anime poster corners preserved
  ....... Manga “Coming Soon” replaced with one-tap switch to manga mode (home & account)
  ....... No ads on manga surfaces (MangaDex AUP)

  Fixed
  ..... Expo Go crash on home tab (expo-notifications guarded import)
  ..... Manga reader settings — page/scroll mode and quality selection apply correctly
```

---

## [2.0.13] - 2026-07-16

```
  versionCode ...... 213

  Fixed
  ..... Production build metadata + public release pipeline sync

  Notes
  ..... New Production Build.
```

---

## [1.1.0] - TBD

```
  versionCode ...... 2 (planned for next public APK publish)

  Added
  ..... Quality / server selection in player settings
  ..... Backend-backed like / dislike counters
  ..... Hardened control lock behavior
  ..... Subtitle safe-area presentation improvements

  Fixed
  ..... Player overlay layout snap artifacts
  ..... Engagement icons cleaned up in landscape bar

  Notes
  ..... Publish this section only when the matching APK is attached to Releases
```

---

## [1.0.0] - Initial public channel

```
  versionCode ...... 1

  Highlights
  .......... First production packaging identity: com.paradis.app
  .......... AniList OAuth-based accounts
  .......... Native episode player with Sub / Dub tracks
  .......... Continue Watching timestamp persistence
  .......... Search with multi-season grouping
  .......... Threaded comments
  .......... Home discovery + My List / Browse tabs
  .......... In-app update plumbing against public version metadata
```

---

## Template for maintainers

```
  ## [X.Y.Z] - YYYY-MM-DD

  versionCode ...... N

  Added
  ..... ...

  Changed
  ....... ...

  Fixed
  ..... ...

  Security
  ........ ...
```

```
 ===============================================================================
  end of CHANGELOG  ::  Paradis
 ===============================================================================
```
