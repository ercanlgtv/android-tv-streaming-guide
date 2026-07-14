# Android TV Streaming Guide

> Everything you need to replace **Stremio** and **CloudStream** on your Android
> TV.  
> Apps, links, features, what supports what — no fluff.

---

## Jump to

- [Stremio Addon Compatible Apps](#-stremio-addon-compatible-apps)
- [CloudStream Plugin Compatible Apps](#-cloudstream-plugin-compatible-apps)
- [All FOSS Alternatives](#-all-foss-alternatives)
- [Hidden Gems Worth Knowing](#-hidden-gems-worth-knowing)
- [Feature Comparison](#-feature-comparison)
- [What Does NOT Support These Addons](#-what-does-not-support-these-addons)
- [Final Recommendations](#-final-recommendations)
- [Ecosystem & Tools](#-ecosystem--tools)

---

## 📺 Stremio Addon Compatible Apps

### Native Support (Paste a Stremio manifest URL and it just works)

| App            | Links                                                                      | Android TV | Key Features                                                                                       |
| -------------- | -------------------------------------------------------------------------- | :--------: | -------------------------------------------------------------------------------------------------- |
| **NuvioTV**    | [GitHub](https://github.com/NuvioMedia/NuvioTV) · [Site](https://nuvio.tv) |     ✅     | Profiles, cross-device sync, MPV player, Trakt, debrid, free (Stremio charges $39/yr for profiles) |
| **ARVIO**      | [GitHub](https://github.com/ProdigyV21/ARVIO) · [Site](https://arvio.tv)   |     ✅     | Unifies Jellyfin + Plex + Emby + Stremio addons + IPTV in one UI. Apache 2.0                       |
| **MediaStorm** | [GitHub](https://github.com/godver3/mediastorm)                            |     ✅     | Stremio addon bundles, debrid, Usenet, Docker self-host. Renamed from STRMR                        |
| **DodoStream** | [GitHub](https://github.com/DodoraApp/DodoStream)                          |     ✅     | Privacy-focused, React Native, works with Stremio addons                                           |
| **Lumera**     | [GitHub](https://github.com/LumeraD3v/Lumera)                              |     ✅     | Import your Stremio account, IntroDb skip intro, adaptive HLS/DASH, speed control                  |
| **Nexio**      | [GitHub](https://github.com/johnneerdael/nexio)                            |     ✅     | Companion web portal for easy setup, debrid-aware, 49 releases in 3 months                         |
| **Debrify**    | [GitHub](https://github.com/varunsalian/debrify)                           | ✅ TV mode | Debrid manager + Stremio addons + built-in mpv player + Jackett/Prowlarr search plugins            |

### Bridge — Run Stremio Addons Inside Another App

| App         | Bridge       | Links                                                                              | How It Works                                                                                                               |
| ----------- | ------------ | ---------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **Kodi**    | Stremio2Kodi | [GitHub](https://github.com/VSeryi/plugin.video.stremio2kodi)                      | Kodi addon that wraps Stremio addons — paste manifest URL, browse in Kodi UI. HDR/DV/IMAX detection, auto-play, TMDbHelper |
| **Syncler** | Providra     | [GitHub](https://github.com/dtankdempsey2/Providra) · [Site](https://providra.com) | Android server that converts Stremio addon responses into Syncler format. Also supports Nuvio plugins                      |
| **Chillio** | ChilliBridge | [GitHub](https://github.com/elfhosted/chillibridge) · [Site](https://chillio.app)  | Apple-only. Server translates Stremio addon → ChillLink protocol. MediaFlow proxy support                                  |

---

## ☁️ CloudStream Plugin Compatible Apps

**Hard truth:** Only **2 non-fork apps** can load native `.cs3` CloudStream
plugins.  
**Why:** `.cs3` files are compiled Kotlin bytecode (DEX) — requires Android's
`DexClassLoader`, GPL-3.0 copyleft, Android-specific APIs.

### Actually Loads .cs3 Files

| App                 | GitHub                                                                                          |         Coverage          | Android TV  |
| ------------------- | ----------------------------------------------------------------------------------------------- | :-----------------------: | :---------: |
| **Sozo (Soplay)**   | [professorDeveloper/sozo](https://github.com/professorDeveloper/sozo)                           |    ~70/73 plugins work    | ✅ Flutter  |
| **cloudstream-web** | [mindflarevortx-maker/cloudstream-web](https://github.com/mindflarevortx-maker/cloudstream-web) | JS ports only (no `.cs3`) | ❌ Web only |

### Feature Requested (Not Implemented)

| App             | Issue                                                        | Request                                                   |
| --------------- | ------------------------------------------------------------ | --------------------------------------------------------- |
| **NuvioMobile** | [#980](https://github.com/NuvioMedia/NuvioMobile/issues/980) | Add repo.json support, CloudStream provider compatibility |

### CloudStream Itself (Still Active — Last Resort)

| Fork                                        | GitHub                                                                             |     Stars     |
| ------------------------------------------- | ---------------------------------------------------------------------------------- | :-----------: |
| **recloudstream/cloudstream** (main)        | [link](https://github.com/recloudstream/cloudstream)                               |    10.1k★     |
| **Stormunblessed**                          | [link](https://github.com/Stormunblessed/cloudstream-3)                            |     131★      |
| **cloudstream3/cs3-android** (new official) | [link](https://github.com/cloudstream3/cs3-android)                                |       —       |
| **Original** (archived)                     | [LagradOst/CloudStream-3](https://codeberg.org/cloudstream/cloudstream) (Codeberg) | Archived 2023 |

### CloudStream Plugin Repos

| Repo               | Link                                                                                          | What's Inside                                                  |
| ------------------ | --------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| **phisher98**      | [cloudstream-extensions-phisher](https://github.com/phisher98/cloudstream-extensions-phisher) | 78 providers, movies/TV/anime/live/torrent/music, 16 languages |
| **MegaRepo**       | [self-similarity/MegaRepo](https://github.com/self-similarity/MegaRepo)                       | Meta-installer — installs all known repos at once              |
| **cs3plugs**       | [justsimplyleon/cs3plugs](https://github.com/justsimplyleon/cs3plugs)                         | Curated list of what actually works                            |
| **CSX**            | [SaurabhKaperwan/CSX](https://github.com/SaurabhKaperwan/CSX)                                 | Extra provider collection                                      |
| **Official repos** | [recloudstream/cs-repos](https://github.com/recloudstream/cs-repos)                           | Official database                                              |

---

## 🧩 All FOSS Alternatives

### All-in-One (Everything in One App)

|                     |                           NuvioTV                           |                          ARVIO                          |                         MediaStorm                          |
| ------------------- | :---------------------------------------------------------: | :-----------------------------------------------------: | :---------------------------------------------------------: |
| **GitHub**          | [NuvioMedia/NuvioTV](https://github.com/NuvioMedia/NuvioTV) | [ProdigyV21/ARVIO](https://github.com/ProdigyV21/ARVIO) | [godver3/mediastorm](https://github.com/godver3/mediastorm) |
| **License**         |                           GPL-3.0                           |                       Apache-2.0                        |                             OSS                             |
| **ATV**             |                          ✅ Native                          |                        ✅ Native                        |                          ✅ Native                          |
| **Stremio addons**  |                           ✅ Full                           |                         ✅ Full                         |                           ✅ Full                           |
| **Trakt**           |                             ✅                              |                           ✅                            |                             ✅                              |
| **Debrid**          |                       ✅ RD/AD/PM/TB                        |                     ✅ RD/AD/PM/TB                      |                       ✅ RD/AD/PM/TB                        |
| **External player** |                           ✅ MPV                            |                           ❌                            |                             ✅                              |
| **Extra**           |               Profiles, sync, cross-platform                |            Also does Jellyfin/Plex/Emby/IPTV            |                       Docker, Usenet                        |

### 🏛️ Media Centers

**Kodi** — [GitHub](https://github.com/xbmc/xbmc) · GPL-2.0 · ✅ Native ATV

- Thousands of Python addons for streaming, scrapers, subtitles, skins
- Stremio addons via Stremio2Kodi bridge
- Supports everything: torrent, debrid, IPTV (PVR), SMB, NFS, WebDAV, UPnP, FTP
- Dolby Atmos / TrueHD passthrough, audio DSP, RetroPlayer gaming
- Heavy but unmatched power

**Jellyfin Android TV** —
[GitHub](https://github.com/jellyfin/jellyfin-androidtv) · GPL-2.0 · ✅ Native
ATV

- Client for self-hosted Jellyfin media server
- Server plugins for Trakt, metadata, subtitles
- External player support (MPV)
- Best FOSS media server ecosystem (52.6k★ on server repo)

### ▶️ Media Players

| App                   | GitHub                                                                    |  License   |     ATV     |  Subs  | Trakt | Protocols               |
| --------------------- | ------------------------------------------------------------------------- | :--------: | :---------: | :----: | :---: | ----------------------- |
| **VLC for ATV**       | [videolan/vlc](https://github.com/videolan/vlc)                           |  LGPL-2.1  |  ✅ Native  | ✅ All |  ❌   | SMB/NFS/UPnP/HTTP/DLNA  |
| **Nova Video Player** | [nova-video-player/aos-AVP](https://github.com/nova-video-player/aos-AVP) |  GPL-3.0   |  ✅ Native  |   ✅   |  ✅   | SMB/NFS/UPnP/WebDAV/FTP |
| **Just Player**       | [moneytoo/Player](https://github.com/moneytoo/Player)                     | Unlicense  | ⚠️ Sideload |   ✅   |  ❌   | File picker             |
| **Next Player**       | [anilbeesetti/nextplayer](https://github.com/anilbeesetti/nextplayer)     | Apache-2.0 | ⚠️ Sideload |   ✅   |  ❌   | File picker/DASH/HLS    |

### ⚡ Debrid-Focused

| App           | GitHub                                                                                      | Debrid Services                   | Highlights                                                                               |
| ------------- | ------------------------------------------------------------------------------------------- | --------------------------------- | ---------------------------------------------------------------------------------------- |
| **Flixorent** | [Hashaleen420/Flixorent](https://github.com/Hashaleen420/Flixorent)                         | RD, AD, Premiumize (beta), TorBox | Built-in Torrentio = zero config. Auto-rank 4K→1080p→720p. Chromecast. Apache 2.0        |
| **Debrify**   | [varunsalian/debrify](https://github.com/varunsalian/debrify)                               | RD, TorBox, PikPak                | Stremio addons + debrid manager + mpv player + Jackett/Prowlarr plugins + download queue |
| **Unchained** | [LivingWithHippos/unchained-android](https://github.com/LivingWithHippos/unchained-android) | RD only                           | Mature (since 2020). F-Droid. Jackett/Prowlarr search. External player. Not TV-optimized |

### 🎬 YouTube (Ad-Free)

| App           | GitHub                                                        |     ATV     | What Makes It Special                                                          |
| ------------- | ------------------------------------------------------------- | :---------: | ------------------------------------------------------------------------------ |
| **SmartTube** | [yuliskov/SmartTube](https://github.com/yuliskov/SmartTube)   |  ✅ Native  | 4K/HDR, SponsorBlock, no ads, return dislikes, background play. The king. 29k★ |
| **Clipious**  | [lamarios/clipious](https://github.com/lamarios/clipious)     |  ✅ Native  | Invidious client, SponsorBlock+DeArrow, audio-only mode, downloads             |
| **SkyTube**   | [SkyTubeTeam/SkyTube](https://github.com/SkyTubeTeam/SkyTube) | ⚠️ Sideload | No Google account needed, no tracking, channel blocklist, OPML                 |

### 📡 IPTV

| App             | GitHub                                                                  |    ATV    | Engine                                   | Features                                                                          |
| --------------- | ----------------------------------------------------------------------- | :-------: | ---------------------------------------- | --------------------------------------------------------------------------------- |
| **OwnTV**       | [ahXN00/OwnTV](https://github.com/ahXN00/OwnTV)                         | ✅ Native | Dual: libmpv (movies) + ExoPlayer (live) | Xtream + M3U, fast switching, beautiful modern UI                                 |
| **Strix**       | [isnow-git/strix](https://github.com/isnow-git/strix)                   | ✅ Native | ExoPlayer                                | Built for low-RAM budget TVs. Clean Compose. Apache 2.0                           |
| **DangoPlayer** | [brunochanrio/DangoPlayer](https://github.com/brunochanrio/DangoPlayer) | ✅ Native | ExoPlayer                                | DRM, PiP, Google Live Channels integration, M3U/PLS                               |
| **Fermata**     | [AndreyPavlenko/Fermata](https://github.com/AndreyPavlenko/Fermata)     | ✅ Native | Pluggable (MP/Exo/VLC)                   | IPTV + EPG, YouTube + SponsorBlock, network folders, CUE sheets. Swiss Army knife |

### 🟣 Twitch

| App               | GitHub                                                        |       ATV       | Features                                                          |
| ----------------- | ------------------------------------------------------------- | :-------------: | ----------------------------------------------------------------- |
| **S0undTV**       | [S0und/S0undTV](https://github.com/S0und/S0undTV)             |    ✅ Native    | Ad-free, chat, BTTV/FFZ/7TV emotes, VOD support                   |
| **SmartTwitchTV** | [fgl27/SmartTwitchTV](https://github.com/fgl27/SmartTwitchTV) |    ✅ Native    | Web-based, on Google Play, lightweight                            |
| **ThystTV**       | [tzii/ThystTV](https://github.com/tzii/ThystTV)               | ✅ Large-screen | Floating chat overlay, watch history stats, Xtra fork with polish |

### 🎌 Anime

| App            | GitHub                                                            |     ATV     | System             | Features                                                                    |
| -------------- | ----------------------------------------------------------------- | :---------: | ------------------ | --------------------------------------------------------------------------- |
| **Aniyomi**    | [aniyomiorg/aniyomi](https://github.com/aniyomiorg/aniyomi)       | ⚠️ Sideload | APK extensions     | MAL/Anilist, MPV/VLC, video + manga. Tachiyomi fork with streaming          |
| **Miru**       | [miru-project/miru-app](https://github.com/miru-project/miru-app) | ⚠️ Sideload | JS extensions      | Video/comics/novels. v2+ has ATV support                                    |
| **Hikari**     | [Hflott/hikari_app](https://github.com/Hflott/hikari_app)         |  ✅ Native  | HAP addon protocol | AniList sync, torrent streaming, batch series packs. Excellent code quality |
| **OpenStream** | [Ivorisnoob/OpenStream](https://github.com/Ivorisnoob/OpenStream) |   ✅ ATV    | HLS via WebView    | Material 3, TMDB metadata, Clean Architecture                               |

### 📊 Tracking

| App                   | GitHub                                                        |    ATV    | Services                                                    |
| --------------------- | ------------------------------------------------------------- | :-------: | ----------------------------------------------------------- |
| **NyanTV**            | [NyanTV/NyanTV](https://github.com/NyanTV/NyanTV)             | ✅ Native | AniList + MyAnimeList + Simkl. Purpose-built for Android TV |
| **Trakt for Android** | [trakt/trakt-android](https://github.com/trakt/trakt-android) | ✅ Native | Official Trakt client for Android + ATV                     |

---

## 💎 Hidden Gems Worth Knowing

Projects under 500★ that punch above their weight.

|  #  | App               |  ★  | What Makes It Special                                                                                             |
| :-: | ----------------- | :-: | ----------------------------------------------------------------------------------------------------------------- |
|  1  | **Nexio**         | 19  | Full Stremio addons + companion web portal + debrid-aware. 49 releases in 3 months. Cross-device sync via web     |
|  2  | **OwnTV**         | 225 | Dual-engine IPTV (libmpv + ExoPlayer). 17 releases in one month. Explosive growth. Beautiful ATV UI               |
|  3  | **Flixorent**     | 90  | Zero-config debrid — built-in Torrentio. Supports RD/AD/PM/TB. Chromecast. Apache 2.0                             |
|  4  | **Hikari**        |  2  | Custom HAP addon protocol for anime torrents. AniList sync. Batch series packs. Engineering quality is stellar    |
|  5  | **NyanTV**        | 64  | Only tracking app purpose-built for Android TV. AniList + MAL + Simkl. Beautiful Compose UI                       |
|  6  | **Strix**         |  0  | Best code quality found. Built for low-RAM TVs. Clean. Apache 2.0                                                 |
|  7  | **JellyPlay**     | new | Most feature-rich Jellyfin client. Triple engine. SyncPlay. Jellyseerr integration. IPTV. Overkill but impressive |
|  8  | **LitPlayer**     | 176 | Supports SMB + WebDAV + FTP + Jellyfin + UPnP. Material 3. Separate TV build. Lite variant for old devices        |
|  9  | **Cineflux**      | new | Native libtorrent4j on ATV. Letterboxd categories. Transmission integration. MIT                                  |
| 10  | **ThystTV**       | 24  | Polish-focused Twitch client. Floating chat. Watch history stats. AGPL-3.0                                        |
| 11  | **Aperture**      |  8  | Brand new Material 3 media player. Compose for TV. Clean. Has a Discord                                           |
| 12  | **Lumera**        | 201 | Full Stremio addons + account import. IntroDb skip. Source switching mid-playback                                 |
| 13  | **Debrify**       | 312 | Stremio addons + debrid manager built-in. Cross-platform. Jackett/Prowlarr search                                 |
| 14  | **Sozo**          | 27  | Only non-fork app that loads CloudStream .cs3 plugins natively. Flutter. ~70/73 plugins work                      |
| 15  | **Laposa Player** |  3  | 30MB. NFS+SMB+SFTP. No cache growth. MIT. Perfect for low-storage TVs                                             |

---

## 🔍 Feature Comparison

| App               |     OS     | ATV |  Remote  |      Stremio Addon      | CS Plugin | Own Plugins  | Trakt | Sync | Ext Player | Subs  |
| ----------------- | :--------: | :-: | :------: | :---------------------: | :-------: | :----------: | :---: | :--: | :--------: | :---: |
| **NuvioTV**       |  GPL-3.0   | ✅  | ⭐⭐⭐⭐ |         ✅ Full         |    ❌     |   Stremio    |  ✅   |  ✅  |   ✅ MPV   |  ✅   |
| **ARVIO**         | Apache-2.0 | ✅  | ⭐⭐⭐⭐ |         ✅ Full         |    ❌     |   Stremio    |  ✅   |  ✅  |     ❌     |  ✅   |
| **MediaStorm**    |    OSS     | ✅  |  ⭐⭐⭐  |         ✅ Full         |    ❌     |   Stremio    |  ✅   |  ✅  |     ✅     |  ✅   |
| **Kodi**          |  GPL-2.0   | ✅  | ⭐⭐⭐⭐ |        ⚠️ Bridge        |    ❌     | 1000s Python |  ✅   |  ✅  |     ✅     |  ✅   |
| **Jellyfin ATV**  |  GPL-2.0   | ✅  | ⭐⭐⭐⭐ |           ❌            |    ❌     | Server plugs |  ✅   |  ✅  |   ✅ MPV   |  ✅   |
| **CloudStream 3** |  GPL-3.0   | ✅  |   ⭐⭐   |        ⚠️ Plugin        |    ✅     |     .cs3     |  ✅   |  ❌  | ✅ MPV/VLC |  ✅   |
| **Flixorent**     | Apache-2.0 | ✅  |  ⭐⭐⭐  | ❌ (built-in Torrentio) |    ❌     |      No      |  ❌   |  ❌  | ✅ VLC/MX  |  ✅   |
| **Debrify**       |   Custom   | ✅  |  ⭐⭐⭐  |         ✅ Full         |    ❌     |   Jackett    |  ✅   |  ❌  |   ✅ mpv   |  ✅   |
| **VLC ATV**       |  LGPL-2.1  | ✅  | ⭐⭐⭐⭐ |           ❌            |    ❌     |      No      |  ❌   |  ❌  |     No     |  ✅   |
| **Nova Player**   |  GPL-3.0   | ✅  |  ⭐⭐⭐  |           ❌            |    ❌     |      No      |  ✅   |  ❌  |     No     |  ✅   |
| **SmartTube**     |    MIT     | ✅  | ⭐⭐⭐⭐ |           ❌            |    ❌     |      No      |  ❌   |  ✅  |     No     | ✅ YT |
| **OwnTV**         |  GPL-3.0   | ✅  | ⭐⭐⭐⭐ |           ❌            |    ❌     |      No      |  ❌   |  ❌  |     No     |  ❌   |
| **Sozo**          |     ❓     | ✅  |   ⭐⭐   |           ❌            |  ✅ Full  |      CS      |  ❌   |  ❌  |     ❓     |  ❓   |
| **Miru**          |  AGPL-3.0  | ⚠️  |   ⭐⭐   |           ❌            |    ❌     |    JS ext    |  ❌   |  ❌  |     No     |  ❌   |

### Debrid Services

| App            | Real-Debrid |  AllDebrid  | Premiumize  |   TorBox    |
| :------------- | :---------: | :---------: | :---------: | :---------: |
| **NuvioTV**    |     ✅      |     ✅      |     ✅      |     ✅      |
| **ARVIO**      |     ✅      |     ✅      |     ✅      |     ✅      |
| **MediaStorm** |     ✅      |     ✅      |     ✅      |     ✅      |
| **Flixorent**  |     ✅      |     ✅      |   ⚠️ Beta   |     ✅      |
| **Debrify**    |     ✅      |     ❌      |     ❌      |     ✅      |
| **Unchained**  |     ✅      |     ❌      |     ❌      |     ❌      |
| **Kodi**       | ✅ (addons) | ✅ (addons) | ✅ (addons) | ✅ (addons) |

### Protocols

| App              |  Torrent  |    IPTV     |    SMB    |    NFS    |  WebDAV   | UPnP |    FTP    |
| :--------------- | :-------: | :---------: | :-------: | :-------: | :-------: | :--: | :-------: |
| **Kodi**         | ✅ addons |   ✅ PVR    |    ✅     |    ✅     |    ✅     |  ✅  |    ✅     |
| **Jellyfin ATV** |    ❌     |  ✅ server  | ✅ server | ✅ server | ✅ server |  ❌  | ✅ server |
| **VLC ATV**      |    ❌     | ✅ playlist |    ✅     |    ❌     |    ✅     |  ✅  |    ❌     |
| **Nova Player**  |    ❌     |     ❌      |    ✅     |    ✅     |    ✅     |  ✅  |    ✅     |
| **LitPlayer**    |    ❌     |     ❌      |    ✅     |    ❌     |    ✅     |  ✅  |    ✅     |
| **Fermata**      |    ❌     |  ✅ addon   |    ✅     |    ❌     |    ❌     |  ❌  |    ✅     |

---

## 🚫 What Does NOT Support These Addons

### No Stremio Addon Support

| App                     | Their System                 | Notes                                               |
| ----------------------- | ---------------------------- | --------------------------------------------------- |
| **CinemaHD**            | Own scrapers                 | Effectively shut down early 2026                    |
| **BeeTV**               | Own scrapers                 | Closed-source                                       |
| **NovaTV**              | Own scrapers                 | Closed-source                                       |
| **CyberFlix**           | Own scrapers                 | Defunct                                             |
| **FilmPlus**            | Own scrapers                 | Closed-source                                       |
| **TeaTV**               | Own scrapers                 | Closed-source                                       |
| **PopcornTime**         | Built-in torrent scraper     | Desktop rewrite active, no ATV                      |
| **HDO Box**             | Own sources                  | Closed-source                                       |
| **OnStream**            | Own sources                  | Declining quality                                   |
| **Weyd**                | Own provider packages        | Proprietary, paid                                   |
| **Plex**                | Deprecated plugin system     | Proprietary                                         |
| **Jellyfin**            | Server plugins               | Bridges exist TO Jellyfin from Stremio, not reverse |
| **Infuse / VidHub**     | Cloud drives / Plex/Jellyfin | No addon system                                     |
| **Flud / LibreTorrent** | None                         | Downloaders only                                    |

### No CloudStream Plugin Support

| App                            | Their System                     | Why Not                     |
| ------------------------------ | -------------------------------- | --------------------------- |
| **Miru**                       | JS extensions                    | Can't load DEX `.cs3` files |
| **Aniyomi**                    | APK extensions (Tachiyomi-style) | Different format            |
| **Stremio**                    | JSON addon manifests             | Different protocol          |
| **Syncler**                    | Vendor packages                  | Proprietary format          |
| **Kodi**                       | Python addons                    | No DEX classloader          |
| **BeeTV / CinemaHD / HDO Box** | None / own scrapers              | No plugin system            |

---

## 🏆 Final Recommendations

### Best Android TV Experience

**ARVIO** — Purpose-built Leanback UI. Jellyfin + Plex + Emby + Stremio addons +
IPTV in one app.  
**NuvioTV** — Also excellent. Free profiles (Stremio charges $39/yr now).

### Best FOSS Project Overall

**Jellyfin** (52.6k★) — Most active, healthiest, most important FOSS media
project. Complete server + ATV client.

### Best Plugin Ecosystem

**Kodi** — Thousands of addons. Stremio2Kodi bridge brings Stremio addons in.
Nothing else is close.

### Best Replacement for Stremio

**NuvioTV** — Full Stremio addon compatibility. Free profiles. Cross-device
sync. MPV. Trakt.  
**ARVIO** — Better if you also use Jellyfin/Plex.

### Best Replacement for CloudStream

**CloudStream 3** (recloudstream) — Still actively maintained (commit today,
10.1k★). No app comes close to its `.cs3` ecosystem. Android TV issues are
acknowledged.  
**Kodi + Stremio2Kodi** — More stable on ATV, uses Stremio addons through
bridge.

### Best Lightweight

**Flixorent** — <70MB. Built-in Torrentio. Zero config. Debrid + P2P. Apache
2.0.

### Best Power-User

**Kodi** — Every protocol. Dolby Atmos passthrough. Audio DSP. RetroPlayer.
PVR/DVR. Endless skins.

### Recommended Combos

```
# One App to Rule Them All
ARVIO → add Jellyfin server + Stremio addon URLs + IPTV playlist

# Stremio Replacement
NuvioTV (movies/TV via Stremio addons) + SmartTube (YouTube)

# Self-Hosted Power
Jellyfin Server → Riven (debrid automation) → ARVIO or Jellyfin ATV → Seerr (requests)

# Budget / Low-End TV
Flixorent (built-in Torrentio + RD, zero config) + SmartTube + OwnTV (IPTV)

# CloudStream Replacement
CloudStream 3 (latest recloudstream) + Phisher repo + StremioX plugin
OR
Kodi + Stremio2Kodi + Stremio addons of choice
```

---

## 🗺️ Ecosystem & Tools

```
                    DEBRID SERVICES
          (Real-Debrid · AllDebrid · Premiumize · TorBox)
                        │
        ┌───────────────┼───────────────┬───────────────┐
        ▼               ▼               ▼               ▼
   DEBRID TOOLS      SCRAPERS       AUTOMATION     TORRENT NATIVE
   RDTClient        Torrentio       Riven          WebTorrent
   Zurg (WebDAV)    Comet           (FUSE VFS)     Fluxstream
   DMM              MediaFusion     Seerr          GoStream
   StremThru        AIOStreams      Sonarr/Radarr  Stream Server
        │               │               │               │
        └───────────────┴───────────────┴───────────────┘
                            │
                      MEDIA SERVERS
              Jellyfin (FOSS) · Plex (ref) · Emby
                            │
                            ▼
                 ANDROID TV FRONTENDS
        All-in-One              Single-Service
        NuvioTV                 Jellyfin ATV
        ARVIO                   SmartTube (YT)
        Kodi                    VLC (local)
        CloudStream 3           OwnTV (IPTV)
        MediaStorm              Nova (local)
        Flixorent               Sozo (CS)
```

### Key Integrations

- **CloudStream 3** runs Stremio addons via StremioX/StremioC plugin (in phisher
  repo)
- **Kodi** runs Stremio addons via Stremio2Kodi bridge
- **Syncler** runs Stremio addons via Providra bridge
- **Riven** mounts FUSE VFS → Jellyfin scans it → automated pipeline
- **Zurg + rclone → Jellyfin** = classic debrid mount stack
- **Comet + StremThru** = unified debrid API for 9 providers
- **ElfHosted** = managed hosting for Comet, MediaFusion, Riven, MediaStorm

### Core Tools

| Tool              | What It Does                                        | Link                                                                 |
| ----------------- | --------------------------------------------------- | -------------------------------------------------------------------- |
| **RDTClient**     | Debrid torrent client proxy                         | [GitHub](https://github.com/rogerfar/rdt-client)                     |
| **Zurg**          | WebDAV for Real-Debrid                              | [GitHub](https://github.com/debridmediamanager/zurg)                 |
| **DMM**           | Debrid Media Manager                                | [GitHub](https://github.com/debridmediamanager/debrid-media-manager) |
| **StremThru**     | Unified debrid API (9 providers)                    | [GitHub](https://github.com/MunifTanjim/stremthru)                   |
| **Comet**         | Stremio addon with multi-debrid                     | [GitHub](https://github.com/g0ldyy/comet)                            |
| **MediaFusion**   | Universal Stremio addon                             | [GitHub](https://github.com/mhdzumair/MediaFusion)                   |
| **Riven**         | Media automation (Plex debrid successor)            | [Site](https://riven.tv)                                             |
| **Seerr**         | Media request manager (Overseerr+Jellyseerr merged) | [Site](https://seerr.dev)                                            |
| **TorrServer**    | DHT torrent HTTP proxy                              | [GitHub](https://github.com/YouROK/TorrServer)                       |
| **Stream Server** | Rust Stremio server replacement                     | [GitHub](https://github.com/perpetus/stream-server)                  |
