# Android TV Streaming Guide

> Everything to replace **Stremio** and **CloudStream** on your Android TV.  
> Pure lists, links, features, what supports what.

---

## Jump to

- [Apps with Stremio Addon Support](#-apps-with-stremio-addon-support)
- [Apps with CloudStream Plugin Support](#-apps-with-cloudstream-plugin-support)
- [Media Centers](#-media-centers)
- [All-in-One Streaming Apps](#-all-in-one-streaming-apps)
- [IPTV Players](#-iptv-players)
- [Debrid Tools & Players](#-debrid-tools--players)
- [Media Players](#-media-players)
- [YouTube / Twitch](#-youtube--twitch-clients)
- [Anime](#-anime)
- [Tracking & Discovery](#-tracking--discovery)
- [Hidden Gems (<500★)](#-hidden-gems-500)
- [What Does NOT Support](#-what-does-not-support)
- [Comparison Table](#-comparison-table)
- [Final Recommendations](#-final-recommendations)
- [Ecosystem Tools](#-ecosystem--tools)

---

## 📺 Apps With Stremio Addon Support

### Native (paste manifest URL, it works)

| App            | GitHub                                                             |              ATV               | Features                                                                          |
| -------------- | ------------------------------------------------------------------ | :----------------------------: | --------------------------------------------------------------------------------- |
| **NuvioTV**    | [NuvioMedia/NuvioTV](https://github.com/NuvioMedia/NuvioTV) 2k★    |               ✅               | Profiles, sync, MPV, Trakt, debrid, free. Stremio charges $39/yr for profiles now |
| **ARVIO**      | [ProdigyV21/ARVIO](https://github.com/ProdigyV21/ARVIO) 583★       |               ✅               | Unifies Jellyfin + Plex + Emby + IPTV + Stremio addons. Apache 2.0                |
| **MediaStorm** | [godver3/mediastorm](https://github.com/godver3/mediastorm) 112★   |               ✅               | Stremio bundles, debrid, Usenet, Docker self-host. Renamed from STRMR             |
| **DodoStream** | [DodoraApp/DodoStream](https://github.com/DodoraApp/DodoStream)    |               ✅               | Privacy-first, React Native                                                       |
| **Lumera**     | [LumeraD3v/Lumera](https://github.com/LumeraD3v/Lumera) 201★       |               ✅               | Stremio account import, IntroDb, adaptive HLS/DASH, speed control                 |
| **Nexio**      | [johnneerdael/nexio](https://github.com/johnneerdael/nexio) 19★    |               ✅               | Companion web portal, debrid-aware, 49 releases in 3 months                       |
| **Debrify**    | [varunsalian/debrify](https://github.com/varunsalian/debrify) 312★ |             ✅ TV              | Debrid manager + Stremio addons + mpv player + Jackett/Prowlarr                   |
| **VortX**      | [VortXTV/VortX](https://github.com/VortXTV/VortX)                  | ❌ (Apple now, Android coming) | Native Apple TV/iOS/Mac player. Android next. Stremio addons planned              |

### Collection-code setup

| App | Website | ATV | Features |
|-----|---------|-----|----------|
| Linkstreams | [Official site](https://linkstreams.app/) | ✅ | Free beta. Stremio-compatible addon collections shared by code; no Linkstreams account. History and settings stay on each device. No content included. |

### Bridge — Run Stremio Addons Inside Another App

| Host App          | Bridge                     | Link                                                                                           | How                                                                            |
| ----------------- | -------------------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| **Kodi**          | Stremio2Kodi               | [VSeryi/plugin.video.stremio2kodi](https://github.com/VSeryi/plugin.video.stremio2kodi)        | Kodi addon, paste manifest URL, browse in Kodi UI. HDR/DV detection            |
| **Syncler**       | Providra                   | [dtankdempsey2/Providra](https://github.com/dtankdempsey2/Providra)                            | Android server, converts Stremio addon → Syncler vendor format                 |
| **Inside4ndroid** | M3U-XCAPI-EPG-IPTV-Stremio | [M3U-XCAPI-EPG-IPTV-Stremio](https://github.com/Inside4ndroid/M3U-XCAPI-EPG-IPTV-Stremio) 148★ | Stremio addon that ingests IPTV M3U/XC/EPG with config UI, caching, multi-user |
| **ElfHosted**     | ChilliBridge               | [elfhosted/chillibridge](https://github.com/elfhosted/chillibridge)                            | Translates Stremio addon → ChillLink for Chillio (Apple only)                  |

---

## ☁️ Apps With CloudStream Plugin Support

**Hard truth:** Only 2 non-fork apps can load native `.cs3` files (Kotlin DEX
bytecode).

| App                 | GitHub                                                                                          |    Loads .cs3?    |    ATV     |
| ------------------- | ----------------------------------------------------------------------------------------------- | :---------------: | :--------: |
| **Sozo (Soplay)**   | [professorDeveloper/sozo](https://github.com/professorDeveloper/sozo) 27★                       | ✅ ~70/73 plugins | ✅ Flutter |
| **cloudstream-web** | [mindflarevortx-maker/cloudstream-web](https://github.com/mindflarevortx-maker/cloudstream-web) | ❌ JS ports only  |   ❌ Web   |

**Requested (not done):**

- **NuvioMobile** [#980](https://github.com/NuvioMedia/NuvioMobile/issues/980) —
  asked for CS plugin support May 2026

**CloudStream itself (still the best bet):**

| Fork                                 |  Stars   | Link                                                     |
| ------------------------------------ | :------: | -------------------------------------------------------- |
| **recloudstream/cloudstream** (main) |  10.1k   | [GitHub](https://github.com/recloudstream/cloudstream)   |
| **cloudstream3/cs3-android**         |   new    | [GitHub](https://github.com/cloudstream3/cs3-android)    |
| **LagradOst original**               | archived | [Codeberg](https://codeberg.org/cloudstream/cloudstream) |

**Plugin repos:**

| Repo          | Link                                                                    | Content                    |
| ------------- | ----------------------------------------------------------------------- | -------------------------- |
| **phisher98** | [link](https://github.com/phisher98/cloudstream-extensions-phisher)     | 78 providers, 16 languages |
| **MegaRepo**  | [self-similarity/MegaRepo](https://github.com/self-similarity/MegaRepo) | Install-all meta repo      |
| **cs3plugs**  | [justsimplyleon/cs3plugs](https://github.com/justsimplyleon/cs3plugs)   | Curated working list       |
| **CSX**       | [SaurabhKaperwan/CSX](https://github.com/SaurabhKaperwan/CSX)           | Extra providers            |

---

## 🏛️ Media Centers

| App                     | GitHub                                                                        |   ★   | License |   ATV    |    Plugins     | Protocols                                                        |
| ----------------------- | ----------------------------------------------------------------------------- | :---: | :-----: | :------: | :------------: | ---------------------------------------------------------------- |
| **Kodi**                | [xbmc/xbmc](https://github.com/xbmc/xbmc)                                     | 20.9k | GPL-2.0 |    ✅    |  1000s Python  | Torrent, IPTV, SMB, NFS, WebDAV, UPnP, HTTP, FTP, Plex, Jellyfin |
| **Jellyfin Android TV** | [jellyfin/jellyfin-androidtv](https://github.com/jellyfin/jellyfin-androidtv) | 4.2k  | GPL-2.0 |    ✅    | Server plugins | Via Jellyfin server (SMB/NFS/WebDAV)                             |
| **Jellyfin Server**     | [jellyfin/jellyfin](https://github.com/jellyfin/jellyfin)                     | 52.6k | GPL-2.0 |    —     | NuGet plugins  | All protocols as media source                                    |
| **CoreELEC**            | [CoreELEC/CoreELEC](https://github.com/CoreELEC/CoreELEC)                     | 1.8k  | GPL-2.0 | OS-level |     Kodi's     | Amlogic TV boxes, Dolby Vision, dual-boot with Android           |

### Jellyfin Android TV Clients

| Client          | GitHub                                                                          |  ★   | Features                                                          |
| --------------- | ------------------------------------------------------------------------------- | :--: | ----------------------------------------------------------------- |
| **Official**    | [jellyfin/jellyfin-androidtv](https://github.com/jellyfin/jellyfin-androidtv)   | 4.2k | Direct Play, transcode, live TV, trickplay                        |
| **Findroid**    | [jarnedemeulemeester/findroid](https://github.com/jarnedemeulemeester/findroid) |  —   | Native Android, Jetpack Compose, phone-first                      |
| **Findroid CE** | [midasvo/findroid-ce](https://github.com/midasvo/findroid-ce)                   |  —   | Bleeding-edge fork, Dolby Vision, subtitle styles                 |
| **Wholphin**    | [damontecres/Wholphin](https://github.com/damontecres/Wholphin)                 | ~500 | Plex-style UI, Android TV native, ExoPlayer                       |
| **JellyPlay**   | [raulshma/jellyplay](https://github.com/raulshma/jellyplay)                     |  —   | Triple engine (Exo/mpv/VLC), SyncPlay, IPTV, downloads            |
| **AFinity**     | [MakD/AFinity](https://github.com/MakD/AFinity)                                 |  —   | Compose + LibMPV, modern UI                                       |
| **Gelli**       | [dkanada/gelli](https://github.com/dkanada/gelli)                               |  —   | Jellyfin music, phone                                             |
| **Sinema**      | [visorcraft/Sinema](https://github.com/visorcraft/Sinema) 24★                   |  —   | **Android TV client for Stash**. D-pad, PIN lock, resume. GPL-3.0 |

---

## 🎬 All-in-One Streaming Apps

Apps with their own scraper/provider system OR built-in streaming (not just
Stremio wrappers).

| App               | GitHub                                                                          |   ★   | License | ATV | Source                                                   |
| ----------------- | ------------------------------------------------------------------------------- | :---: | :-----: | :-: | -------------------------------------------------------- |
| **CloudStream 3** | [recloudstream/cloudstream](https://github.com/recloudstream/cloudstream)       | 10.1k | GPL-3.0 | ✅  | .cs3 plugins + StremioX bridge                           |
| **Cinema-HQ**     | [Inside4ndroid/Cinema-HQ](https://github.com/Inside4ndroid/Cinema-HQ) 50★       |   —   |    —    | ✅  | Movies, TV, Live TV, XXX. Own scrapers. Active Jul 2026  |
| **flixquest**     | [BeamlakAschalew/flixquest](https://github.com/BeamlakAschalew/flixquest)       |  344  | GPL-3.0 | ⚠️  | Flutter, movies+TV, open source                          |
| **Tokeii**        | [Sovan22/Tokeii](https://github.com/Sovan22/Tokeii)                             |  159  |    —    | ✅  | Kotlin, movie/TV streaming. Last push Mar 2024 (stale)   |
| **youplex**       | [steveyout/youplex-apk](https://github.com/steveyout/youplex-apk)               |  35   |    —    | ✅  | Cross-platform (Android/iOS/ATV)                         |
| **moviedog**      | [ratanparai/moviedog](https://github.com/ratanparai/moviedog)                   |  21   |    —    | ✅  | Free movie streaming for Android TV                      |
| **Streamflix**    | [streamflix-reborn/streamflix](https://github.com/streamflix-reborn/streamflix) |  712  |    —    | ✅  | Scraper-based, own sources                               |
| **Cinetry**       | [gstory0404/Cinetry](https://github.com/gstory0404/Cinetry)                     | 300+  |    —    | ✅  | Jellyfin + Emby + IPTV + Webdav + CMS. Cross-platform    |
| **GhostenPlayer** | [GhostenEditor/Ghosten-Player](https://github.com/GhostenEditor/Ghosten-Player) | 800+  |    —    | ✅  | Cloud drive + IPTV + metadata scraping + file management |

### Inside4ndroid Ecosystem

| Project                        | GitHub                                                                                                  |  ★  | What It Does                                                                                          |
| ------------------------------ | ------------------------------------------------------------------------------------------------------- | :-: | ----------------------------------------------------------------------------------------------------- |
| **Cinema-HQ**                  | [Inside4ndroid/Cinema-HQ](https://github.com/Inside4ndroid/Cinema-HQ)                                   | 50  | Android streaming app with movies, TV, live TV. Own scrapers                                          |
| **TMDB-Embed-API**             | [Inside4ndroid/TMDB-Embed-API](https://github.com/Inside4ndroid/TMDB-Embed-API)                         | 121 | Streaming metadata + source aggregation API. Plugin system with providers (ShowBox, Vidsrc, etc). MIT |
| **M3U-XCAPI-EPG-IPTV-Stremio** | [Inside4ndroid/M3U-XCAPI-EPG-IPTV-Stremio](https://github.com/Inside4ndroid/M3U-XCAPI-EPG-IPTV-Stremio) | 148 | Stremio addon: IPTV M3U/XC/EPG with config UI, LRU+Redis caching, multi-user                          |
| **ResolveURL**                 | [Inside4ndroid/ResolveURL](https://github.com/Inside4ndroid/ResolveURL)                                 |  —  | Fork of UrlResolver for XBMC/Kodi. GPL-2.0                                                            |
| **zyphera-plugins**            | [Inside4ndroid/zyphera-plugins](https://github.com/Inside4ndroid/zyphera-plugins)                       |  —  | Plugin repo for Zyphera streaming app                                                                 |

---

## 📡 IPTV Players

### Actively Maintained

| App                        | GitHub                                                                                  |  ★   |  ATV   |      Engine       | Features                                                             |
| -------------------------- | --------------------------------------------------------------------------------------- | :--: | :----: | :---------------: | -------------------------------------------------------------------- |
| **mytv-android**           | [mytv-android/mytv-android](https://github.com/mytv-android/mytv-android)               | 2.4k |   ✅   |  Media3/IJK/VLC   | Material 3, Leanback, full IPTV                                      |
| **xplayer**                | [TNT-Likely/xplayer](https://github.com/TNT-Likely/xplayer)                             | 1k+  |   ✅   |     ExoPlayer     | Flutter, Android/iOS/macOS/Win, EPG, iptv-org sources                |
| **Extreme-InfiniTV**       | [infinitel8p/Extreme-InfiniTV](https://github.com/infinitel8p/Extreme-InfiniTV)         | 500+ |   ✅   |         —         | Xtream + M3U, EPG, offline downloads. Cross-platform                 |
| **M3UAndroid**             | [oxyroid/M3UAndroid](https://github.com/oxyroid/M3UAndroid)                             | 500+ |   ✅   |         —         | Clean, ad-free, simple                                               |
| **OwnTV**                  | [ahXN00/OwnTV](https://github.com/ahXN00/OwnTV)                                         | 225  |   ✅   | Dual (libmpv+Exo) | Beautiful UI, 17 releases in first month                             |
| **ultra-tv**               | [khalilbenaz/ultra-tv](https://github.com/khalilbenaz/ultra-tv)                         |  40  |   ✅   |         —         | Xtream, M3U, Stalker. HLS/DASH/MPEG-TS. EPG, DVR, Cast               |
| **Prysm**                  | [dereferencex/prysm](https://github.com/dereferencex/prysm)                             |  30  |   ✅   |     ExoPlayer     | React Native, lightweight, M3U                                       |
| **CosmiTV**                | [cosmiquest/CosmiTV](https://github.com/cosmiquest/CosmiTV)                             | ~100 |   ✅   |     ExoPlayer     | IPTV DVR: rewind/FF live TV, schedule recordings. Stalker/Xtream/M3U |
| **StreamVault-IPTV**       | [Davidona/StreamVault-IPTV](https://github.com/Davidona/StreamVault-IPTV)               | ~100 |   ✅   |      Media3       | Kotlin + Compose + Room + Hilt. TV-first                             |
| **Fermata**                | [AndreyPavlenko/Fermata](https://github.com/AndreyPavlenko/Fermata)                     | 500+ |   ✅   |     Plugable      | IPTV+EPG, YouTube+SponsorBlock, network folders, pluggable engines   |
| **DangoPlayer**            | [brunochanrio/DangoPlayer](https://github.com/brunochanrio/DangoPlayer)                 | ~200 |   ✅   |     ExoPlayer     | IPTV + PiP + Live Channels integration + DRM                         |
| **PipTV**                  | [juniorbarrigana/PipTV](https://github.com/juniorbarrigana/PipTV)                       |  20  | ✅ PiP |      Media3       | M3U/HLS + YouTube floating overlay. Compose for TV                   |
| **foss-tv-player-android** | [jaime-grj/foss-tv-player-android](https://github.com/jaime-grj/foss-tv-player-android) | ~50  |   ✅   |         —         | Live streams from JSON config. Leanback UI                           |
| **Strix**                  | [isnow-git/strix](https://github.com/isnow-git/strix)                                   |  0   |   ✅   |     ExoPlayer     | Built for low-RAM budget TVs. Apache 2.0. Excellent code             |
| **ChuchPlayer**            | [avalos010/ChuchPlayer](https://github.com/avalos010/ChuchPlayer)                       | ~50  |   ✅   |     ExoPlayer     | M3U/Xtream, EPG, catchup                                             |

### Chinese IPTV Apps (Popular but non-English)

| App              | GitHub                                                                |  ★   | Notes                             |
| ---------------- | --------------------------------------------------------------------- | :--: | --------------------------------- |
| **my-tv**        | [lizongying/my-tv](https://github.com/lizongying/my-tv)               | 5k+  | Chinese live TV, install and play |
| **my-tv-0**      | [lizongying/my-tv-0](https://github.com/lizongying/my-tv-0)           | 2k+  | Custom video sources              |
| **easy_tv_live** | [aiyakuaile/easy_tv_live](https://github.com/aiyakuaile/easy_tv_live) | 200+ | Lightweight IPTV, cross-platform  |

---

## ⚡ Debrid Tools & Players

| App                     | GitHub                                                                                                |  ★   |      Debrid      | Features                                                              |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | :--: | :--------------: | --------------------------------------------------------------------- |
| **Flixorent**           | [Hashaleen420/Flixorent](https://github.com/Hashaleen420/Flixorent)                                   |  90  | RD/AD/PM/TorBox  | Built-in Torrentio. Zero config. Chromecast. P2P fallback. Apache 2.0 |
| **Debrify**             | [varunsalian/debrify](https://github.com/varunsalian/debrify)                                         | 312  | RD/TorBox/PikPak | Stremio addons + mpv + download queue + Jackett/Prowlarr              |
| **Unchained**           | [LivingWithHippos/unchained-android](https://github.com/LivingWithHippos/unchained-android)           | 618  |     RD only      | F-Droid, Jackett/Prowlarr, mature (since 2020), not TV-optimized      |
| **RDTClient**           | [rogerfar/rdt-client](https://github.com/rogerfar/rdt-client)                                         |  —   |     RD/AD/TB     | Debrid torrent proxy, Web UI                                          |
| **Zurg**                | [debridmediamanager/zurg](https://github.com/debridmediamanager/zurg)                                 |  —   |        RD        | WebDAV for debrid, mount via rclone                                   |
| **DMM**                 | [debridmediamanager/debrid-media-manager](https://github.com/debridmediamanager/debrid-media-manager) | 1.4k |     RD/AD/TB     | Web app, download to cloud, no storage limits                         |
| **StremThru**           | [MunifTanjim/stremthru](https://github.com/MunifTanjim/stremthru)                                     |  —   |   9 providers    | Unified debrid API                                                    |
| **Debrid Media Bridge** | (community)                                                                                           |  —   |     RD/AD/PM     | Bridges debrid to media apps                                          |
| **elfhosted**           | [ElfHosted](https://elfhosted.com)                                                                    |  —   |       All        | Managed hosting for debrid stack                                      |

---

## ▶️ Media Players

| App                   | GitHub                                                                    |   ★   | ATV |  Subs  | Trakt | Protocols                    |
| --------------------- | ------------------------------------------------------------------------- | :---: | :-: | :----: | :---: | ---------------------------- |
| **VLC for ATV**       | [videolan/vlc](https://github.com/videolan/vlc)                           | 16.1k | ✅  | ✅ All |  ❌   | SMB/NFS/UPnP/HTTP/DLNA       |
| **Nova Video Player** | [nova-video-player/aos-AVP](https://github.com/nova-video-player/aos-AVP) | 4.5k  | ✅  |   ✅   |  ✅   | SMB/NFS/UPnP/WebDAV/FTP      |
| **Just Player**       | [moneytoo/Player](https://github.com/moneytoo/Player)                     | 2.5k  | ⚠️  |   ✅   |  ❌   | File picker                  |
| **Next Player**       | [anilbeesetti/nextplayer](https://github.com/anilbeesetti/nextplayer)     | 4.1k  | ⚠️  |   ✅   |  ❌   | File picker/DASH/HLS         |
| **LitPlayer**         | [daluobo/LitPlayer-release](https://github.com/daluobo/LitPlayer-release) |  176  | ✅  |   ✅   |  ❌   | SMB/WebDAV/FTP/Jellyfin/UPnP |
| **Aperture**          | [XDanfr/Aperture](https://github.com/XDanfr/Aperture)                     |   8   | ✅  |   ✅   |  ❌   | Media3/ExoPlayer. M3-themed  |

---

## 🎬 YouTube / Twitch Clients

| App               | GitHub                                                        |  ★   | ATV | What                                       |
| ----------------- | ------------------------------------------------------------- | :--: | :-: | ------------------------------------------ |
| **SmartTube**     | [yuliskov/SmartTube](https://github.com/yuliskov/SmartTube)   | 29k  | ✅  | 4K/HDR, SponsorBlock, no ads. The king     |
| **Clipious**      | [lamarios/clipious](https://github.com/lamarios/clipious)     | 1k+  | ✅  | Invidious client, SponsorBlock+DeArrow     |
| **SkyTube**       | [SkyTubeTeam/SkyTube](https://github.com/SkyTubeTeam/SkyTube) | 2.7k | ⚠️  | No Google account, no tracking             |
| **S0undTV**       | [S0und/S0undTV](https://github.com/S0und/S0undTV)             | 2k+  | ✅  | Twitch: ad-free, chat, BTTV/FFZ/7TV        |
| **SmartTwitchTV** | [fgl27/SmartTwitchTV](https://github.com/fgl27/SmartTwitchTV) | 1k+  | ✅  | Twitch web client on Google Play           |
| **ThystTV**       | [tzii/ThystTV](https://github.com/tzii/ThystTV)               |  24  | ✅  | Improved Xtra fork, floating chat AGPL-3.0 |

---

## 🎌 Anime

| App            | GitHub                                                            |  ★   | ATV | Engine                                               |
| -------------- | ----------------------------------------------------------------- | :--: | :-: | ---------------------------------------------------- |
| **Aniyomi**    | [aniyomiorg/aniyomi](https://github.com/aniyomiorg/aniyomi)       | 5k+  | ⚠️  | APK extensions, MAL/Anilist, MPV/VLC                 |
| **Miru**       | [miru-project/miru-app](https://github.com/miru-project/miru-app) | 5.5k | ⚠️  | JS extensions, v2+ ATV                               |
| **Hikari**     | [Hflott/hikari_app](https://github.com/Hflott/hikari_app)         |  2   | ✅  | HAP addon protocol, torrent, AniList. Excellent code |
| **Saikou**     | [saikou-app/saikou](https://github.com/saikou-app/saikou)         |  —   | ⚠️  | Anime + manga                                        |
| **OpenStream** | [Ivorisnoob/OpenStream](https://github.com/Ivorisnoob/OpenStream) |  7   | ✅  | Material 3, TMDB, Clean Architecture                 |
| **MiruShin**   | [emp0ry/MiruShin](https://github.com/emp0ry/MiruShin)             |  —   | ✅  | Flutter, AniList/MAL/Shikimori, AniSkip, PiP         |
| **Dantotsu**   | (check)                                                           |  —   | ⚠️  | Anilist-focused Tachiyomi fork                       |

---

## 📊 Tracking & Discovery

| App               | GitHub                                                        |  ★  | ATV | Services                                       |
| ----------------- | ------------------------------------------------------------- | :-: | :-: | ---------------------------------------------- |
| **NyanTV**        | [NyanTV/NyanTV](https://github.com/NyanTV/NyanTV)             | 64  | ✅  | AniList + MAL + Simkl. Only ATV-native tracker |
| **Trakt Android** | [trakt/trakt-android](https://github.com/trakt/trakt-android) | 43  | ✅  | Official Trakt client for ATV                  |

---

## 💎 Hidden Gems (<500★)

Projects that deserve attention but are under the radar.

|  #  | App                        |  ★   | Why It's Special                                                          |
| :-: | -------------------------- | :--: | ------------------------------------------------------------------------- |
|  1  | **Nexio**                  |  19  | Stremio addons + web portal + debrid. 49 releases in 3mo. Insane velocity |
|  2  | **OwnTV**                  | 225  | Dual-engine IPTV. Explosive growth. Beautiful                             |
|  3  | **Flixorent**              |  90  | Zero-config debrid. Built-in Torrentio. Chromecast                        |
|  4  | **Hikari**                 |  2   | Custom HAP protocol for anime torrents. Stellar code quality              |
|  5  | **NyanTV**                 |  64  | Only ATV-native tracker. AniList/MAL/Simkl                                |
|  6  | **Strix**                  |  0   | Best code quality found. Low-RAM TV focus. Apache 2.0                     |
|  7  | **JellyPlay**              | new  | Most feature-rich Jellyfin client. Triple engine. SyncPlay                |
|  8  | **LitPlayer**              | 176  | Everything: SMB/WebDAV/FTP/Jellyfin/UPnP. Separate TV build               |
|  9  | **Cineflux**               | new  | Native libtorrent4j on ATV. Letterboxd categories                         |
| 10  | **ThystTV**                |  24  | Polish-focused Twitch. AGPL-3.0. Floating chat                            |
| 11  | **Aperture**               |  8   | New M3 media player. Compose for TV. Clean                                |
| 12  | **Lumera**                 | 201  | Full Stremio addons + account import + IntroDb                            |
| 13  | **Sozo**                   |  27  | Only non-fork CS .cs3 loader. ~70/73 plugins work                         |
| 14  | **Sinema**                 |  24  | Stash client for ATV. D-pad, PIN, resume. GPL-3.0                         |
| 15  | **Cinema-HQ**              |  50  | Own scrapers, movies/TV/live. Active Jul 2026                             |
| 16  | **flixquest**              | 344  | Flutter open-source streaming. GPL-3.0                                    |
| 17  | **Prysm**                  |  30  | React Native IPTV. Clean. Lightweight                                     |
| 18  | **StreamVault-IPTV**       | ~100 | Compose + Room + Hilt + Media3. TV-first                                  |
| 19  | **DangoPlayer**            | 200  | IPTV + PiP + Live Channels. Single-dev passion project                    |
| 20  | **foss-tv-player-android** | ~50  | Simple live TV from JSON config. Leanback                                 |

---

## 🚫 What Does NOT Support

### No Stremio Addon Support

| App                                       | Their System             | Notes                              |
| ----------------------------------------- | ------------------------ | ---------------------------------- |
| **CinemaHD**                              | Own scrapers             | Shut down early 2026               |
| **BeeTV / NovaTV / FilmPlus / CyberFlix** | Own scrapers             | Closed-source                      |
| **TeaTV**                                 | Own scrapers             | Closed-source                      |
| **PopcornTime**                           | Built-in torrent scraper | Desktop rewrite only, no ATV       |
| **HDO Box / OnStream**                    | Own sources              | Declining quality                  |
| **Weyd**                                  | Provider packages        | Proprietary, paid                  |
| **Plex**                                  | Deprecated plugins       | Proprietary                        |
| **Jellyfin / Emby**                       | Server plugins           | Bridges exist TO them, not reverse |
| **Infuse / VidHub**                       | Cloud drives / Plex      | No addon system                    |
| **Flud / LibreTorrent**                   | None                     | Downloaders only                   |
| **VLC / Nova Player / Just Player**       | None                     | Local media players only           |

### No CloudStream Plugin Support

| App                              | Their System    | Why                |
| -------------------------------- | --------------- | ------------------ |
| **Miru**                         | JS extensions   | Can't load DEX     |
| **Aniyomi**                      | APK extensions  | Different format   |
| **Stremio**                      | JSON manifests  | Different protocol |
| **Syncler**                      | Vendor packages | Proprietary        |
| **Kodi**                         | Python addons   | No DEX classloader |
| **Tokeii / flixquest / youplex** | Own scrapers    | Not CS-compatible  |

---

## 🔍 Comparison Table

| App               |     OS     | ATV |  Remote  | Stremio Addon | CS Plugin | Trakt | Ext Player | Subs  |    Debrid    |
| ----------------- | :--------: | :-: | :------: | :-----------: | :-------: | :---: | :--------: | :---: | :----------: |
| **NuvioTV**       |  GPL-3.0   | ✅  | ⭐⭐⭐⭐ |      ✅       |    ❌     |  ✅   |   ✅ MPV   |  ✅   | RD/AD/PM/TB  |
| **ARVIO**         | Apache-2.0 | ✅  | ⭐⭐⭐⭐ |      ✅       |    ❌     |  ✅   |     ❌     |  ✅   | RD/AD/PM/TB  |
| **MediaStorm**    |    OSS     | ✅  |  ⭐⭐⭐  |      ✅       |    ❌     |  ✅   |     ✅     |  ✅   | RD/AD/PM/TB  |
| **Kodi**          |  GPL-2.0   | ✅  | ⭐⭐⭐⭐ |   ⚠️ bridge   |    ❌     |  ✅   |     ✅     |  ✅   |  ✅ addons   |
| **Jellyfin ATV**  |  GPL-2.0   | ✅  | ⭐⭐⭐⭐ |      ❌       |    ❌     |  ✅   |   ✅ MPV   |  ✅   |      ❌      |
| **CloudStream 3** |  GPL-3.0   | ✅  |   ⭐⭐   |   ⚠️ plugin   |    ✅     |  ✅   | ✅ MPV/VLC |  ✅   |  ⚠️ limited  |
| **Cinema-HQ**     |     —      | ✅  |   ⭐⭐   |      ❌       |    ❌     |  ❌   |     ❌     |  ❌   |      ❌      |
| **flixquest**     |  GPL-3.0   | ⚠️  |   ⭐⭐   |      ❌       |    ❌     |  ❌   |     ❌     |  ❌   |      ❌      |
| **Flixorent**     | Apache-2.0 | ✅  |  ⭐⭐⭐  | ❌(built-in)  |    ❌     |  ❌   | ✅ VLC/MX  |  ✅   | RD/AD/PM/TB  |
| **Debrify**       |   Custom   | ✅  |  ⭐⭐⭐  |      ✅       |    ❌     |  ✅   |   ✅ mpv   |  ✅   | RD/TB/PikPak |
| **Sozo**          |     ❓     | ✅  |   ⭐⭐   |      ❌       |    ✅     |  ❌   |     ❓     |  ❓   |      ❌      |
| **VLC ATV**       |  LGPL-2.1  | ✅  | ⭐⭐⭐⭐ |      ❌       |    ❌     |  ❌   |     No     |  ✅   |      ❌      |
| **Nova Player**   |  GPL-3.0   | ✅  |  ⭐⭐⭐  |      ❌       |    ❌     |  ✅   |     No     |  ✅   |      ❌      |
| **SmartTube**     |    MIT     | ✅  | ⭐⭐⭐⭐ |      ❌       |    ❌     |  ❌   |     No     | ✅ YT |      ❌      |
| **OwnTV**         |  GPL-3.0   | ✅  | ⭐⭐⭐⭐ |      ❌       |    ❌     |  ❌   |     No     |  ❌   |      ❌      |

---

## 🏆 Final Recommendations

### Best Android TV Experience

→ **ARVIO** — Jellyfin + Plex + Emby + Stremio addons + IPTV. One UI. Apache
2.0.  
→ **NuvioTV** — Stremio addons, free profiles, MPV, sync.

### Best Replacement for Stremio

→ **NuvioTV** — Full Stremio compat. Free profiles (Stremio now $39/yr).  
→ **ARVIO** — Better if you also use Jellyfin/Plex.

### Best Replacement for CloudStream

→ **CloudStream 3** (recloudstream) — Still active. Nothing else loads .cs3.  
→ **Kodi + Stremio2Kodi** — More stable on ATV, uses Stremio addons.

### Best Plugin Ecosystem

→ **Kodi** — Thousands of addons + Stremio2Kodi bridge.

### Best FOSS Project

→ **Jellyfin** (52.6k★) — Healthiest OSS media project.

### Best Lightweight

→ **Flixorent** — <70MB, built-in Torrentio, zero config.

### Best Power-User

→ **Kodi** — Every protocol, Atmos passthrough, RetroPlayer, PVR/DVR.

### Best Hidden Gem

→ **Nexio** — 19★ but 49 releases in 3mo. Stremio + web portal + debrid.

### Best New Discovery

→ **Sinema** (visorcraft/Sinema) — Stash client for Android TV. 24★. GPL-3.0.  
→ **Cinema-HQ** (Inside4ndroid/Cinema-HQ) — 50★, own scrapers, live TV. Active.

### Recommended Combos

```
# One App
ARVIO → Jellyfin/Plex + Stremio addon URLs + IPTV playlist

# Stremio Replacement
NuvioTV + SmartTube

# Self-Hosted Power
Jellyfin Server → Riven (debrid) → ARVIO → Seerr (requests)

# Budget TV
Flixorent (zero config debrid) + SmartTube + OwnTV (IPTV)

# CloudStream
CloudStream 3 (latest) + Phisher repo + StremioX plugin
OR Kodi + Stremio2Kodi + Stremio addons
```

---

## ⚙️ Media Automation & Backend Tools

Backend services that power your Android TV setup — request management, *arr
automation, debrid, and indexing.

### Request Management

| Project        | GitHub                                                              |   ★   | What It Does                                                                                                            |
| -------------- | ------------------------------------------------------------------- | :---: | ----------------------------------------------------------------------------------------------------------------------- |
| **Seerr**      | [seerr-team/seerr](https://github.com/seerr-team/seerr)             | 11.6k | Unified media request manager. Merger of Overseerr + Jellyseerr. Supports Jellyfin, Plex, Emby. Web UI, mobile-friendly |
| **Overseerr**  | [sct/overseerr](https://github.com/sct/overseerr)                   |  5k   | Original Plex request manager. **Archived Feb 2026** — superseded by Seerr                                              |
| **Jellyseerr** | [fallenbagel/jellyseerr](https://github.com/fallenbagel/jellyseerr) |   —   | Jellyfin/Emby fork of Overseerr. Merged into Seerr                                                                      |

### Torrent Indexing

| Project      | GitHub                                                    |   ★   | What It Does                                                                  |
| ------------ | --------------------------------------------------------- | :---: | ----------------------------------------------------------------------------- |
| **Jackett**  | [Jackett/Jackett](https://github.com/Jackett/Jackett)     | 15.6k | API proxy for 500+ torrent trackers. Converts to Torznab API. C#. Very active |
| **Prowlarr** | [Prowlarr/Prowlarr](https://github.com/Prowlarr/Prowlarr) |   —   | Sonarr-style indexer manager. Built-in NZB/torrent support                    |
| **doorr**    | [Lifailon/doorr](https://github.com/Lifailon/doorr)       |  new  | **✅ Android TV** — search frontend for Prowlarr/Jackett. Flutter/Dart        |

### *arr Mobile Clients (Direct Android TV Apps)

| App            | GitHub                                                            | Services                                                                   | Notes                                     |
| -------------- | ----------------------------------------------------------------- | -------------------------------------------------------------------------- | ----------------------------------------- |
| **seekarr**    | [matthw-labs/seekarr](https://github.com/matthw-labs/seekarr)     | Seerr + Radarr + Sonarr + Lidarr + qBittorrent                             | Flutter, APK available                    |
| **arr-client** | [Nicktronix/arr-client](https://github.com/Nicktronix/arr-client) | Sonarr & Radarr                                                            | Material Design 3, Android APK            |
| **uniarr**     | [raulshma/uniarr](https://github.com/raulshma/uniarr)             | Sonarr, Radarr, Jellyseerr, qBittorrent, Jellyfin, Prowlarr, Bazarr, +more | React Native, 15+ services, offline-first |
| **deckarr**    | [iregados/deckarr](https://github.com/iregados/deckarr)           | Radarr, Sonarr, Transmission                                               | Kotlin Multiplatform, Jetpack Compose     |

### Debrid Automation

| Project            | GitHub                                                                                                |   ★    | What It Does                                                                                                           |
| ------------------ | ----------------------------------------------------------------------------------------------------- | :----: | ---------------------------------------------------------------------------------------------------------------------- |
| **Riven**          | [rivenmedia/riven](https://github.com/rivenmedia/riven)                                               | active | Plex/Jellyfin/Emby debrid streaming. FUSE VFS. Scrapers: Comet, Jackett, Prowlarr, Torrentio. Successor to plex_debrid |
| **Riven Frontend** | [rivenmedia/riven-frontend](https://github.com/rivenmedia/riven-frontend)                             | active | Web UI for Riven                                                                                                       |
| **Riven TS**       | [rivenmedia/riven-ts](https://github.com/rivenmedia/riven-ts)                                         | active | TypeScript plugins for Riven                                                                                           |
| **plex_debrid**    | [itsToggle/plex_debrid](https://github.com/itsToggle/plex_debrid)                                     |  1.6k  | **Archived.** Superseded by Riven                                                                                      |
| **rdt-client**     | [rogerfar/rdt-client](https://github.com/rogerfar/rdt-client)                                         | large  | RD/AD/PM/TorBox/DebridLink torrent client. Fake qBittorrent API for *arr. Angular + .NET                               |
| **Zurg**           | [debridmediamanager/zurg-testing](https://github.com/debridmediamanager/zurg-testing)                 | large  | Real-Debrid WebDAV server. Mount as filesystem for Plex/Jellyfin via rclone                                            |
| **DMM**            | [debridmediamanager/debrid-media-manager](https://github.com/debridmediamanager/debrid-media-manager) |  1.4k  | Curate infinite media library. Search/download to RD/AD/TorBox. Stremio + Trakt integration                            |

### Tracking & Discovery (Android)

| App               | GitHub                                                                |  ★  | Services              | Notes                                      |
| ----------------- | --------------------------------------------------------------------- | :-: | --------------------- | ------------------------------------------ |
| **Trakt Android** | [trakt/trakt-android](https://github.com/trakt/trakt-android)         | 35  | Trakt                 | **✅ Official Android TV client**. GPL-3.0 |
| **Showly**        | [michaldrabik/showly-2.0](https://github.com/michaldrabik/showly-2.0) | 1k  | Trakt                 | Modern OSS, no Google services. Kotlin     |
| **NyanTV**        | [NyanTV/NyanTV](https://github.com/NyanTV/NyanTV)                     | 64  | AniList + MAL + Simkl | **✅ Only ATV-native multi-tracker**       |

---

## 🗺️ Full Ecosystem Map

```
DEBRID: Real-Debrid · AllDebrid · Premiumize · TorBox · DebridLink
  ↓
SCRAPERS: Torrentio · Comet · MediaFusion · AIOStreams · Magnetio · Jackettio
  ↓
INDEXERS: Jackett (500 trackers) · Prowlarr · doorr (Android search frontend)
  ↓
BACKEND:
  Debrid:  RDTClient · Zurg (WebDAV) · DMM · StremThru · ElfHosted
  *arr:    Sonarr · Radarr · Lidarr · Bazarr · Readarr
  Mobile:  seekarr · arr-client · uniarr · deckarr
  ↓
AUTOMATION: Riven (FUSE VFS debrid → Plex/Jellyfin)
  REQUEST:  Seerr (Overseerr + Jellyseerr merged)
  ↓
SERVERS: Jellyfin · Plex (ref) · Emby · Kodi (direct)
  ↓
FRONTENDS:
  All-in-One: NuvioTV · ARVIO · Kodi · CloudStream 3 · MediaStorm · Cinema-HQ
  Single:     Jellyfin ATV · SmartTube · VLC · Nova · OwnTV · Flixorent
  IPTV:       mytv-android · xplayer · Extreme-InfiniTV · OwnTV · ultra-tv
  Anime:      Aniyomi · Miru · Hikari
  Tracking:   NyanTV · Trakt Android · Showly

KEY INTEGRATIONS:
  CloudStream 3 → Stremio addons via StremioX plugin (phisher repo)
  Kodi         → Stremio addons via Stremio2Kodi bridge
  Syncler      → Stremio addons via Providra bridge
  Riven        → FUSE VFS → Jellyfin scans as library
  Zurg         → rclone → Jellyfin (classic debrid mount)
  Comet + StremThru → unified debrid API (9 providers)
  Seerr        → Radarr/Sonarr → Riven → Jellyfin/Plex (request → automate → stream)
  doorr        → Prowlarr/Jackett → download on Android (search anywhere)
```

---

> **Research:** July 14, 2026 · 15 parallel GitHub search agents · 100+ repos
> analyzed  
> **Repo:** [github.com/thegnsme/android-tv-streaming-guide](https://github.com/thegnsme/android-tv-streaming-guide)
