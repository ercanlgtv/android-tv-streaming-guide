# Best FOSS Alternatives — Android TV

## ALL-IN-ONE (Stremio + Jellyfin + Plex + IPTV)

| App            | GitHub                                                      | License    | Android TV | Stremio Addons | CS Plugins     | Own Plugins    | Trakt | Ext Player | Subs | Local | Streaming                              |
| -------------- | ----------------------------------------------------------- | ---------- | ---------- | -------------- | -------------- | -------------- | ----- | ---------- | ---- | ----- | -------------------------------------- |
| **ARVIO**      | [ProdigyV21/ARVIO](https://github.com/ProdigyV21/ARVIO)     | Apache-2.0 | ✅ Native  | ✅ Full        | ❌             | Stremio addons | ✅    | ❌         | ✅   | ❌    | Jellyfin/Plex/Emby/Stremio addons/IPTV |
| **NuvioTV**    | [NuvioMedia/NuvioTV](https://github.com/NuvioMedia/NuvioTV) | GPL-3.0    | ✅ Native  | ✅ Full        | ❌ (requested) | Stremio addons | ✅    | ✅ MPV     | ✅   | ❌    | Torrent/Debrid/Stremio addons          |
| **MediaStorm** | [godver3/mediastorm](https://github.com/godver3/mediastorm) | OSS        | ✅ Native  | ✅ Full        | ❌             | Stremio addons | ✅    | ✅         | ✅   | ❌    | Torrent/Debrid/Usenet                  |

## MEDIA CENTERS

| App                     | GitHub                                                                        | License | ATV       | Plugins             | Trakt       | Ext Player | Subs | Local                  | Streaming                         |
| ----------------------- | ----------------------------------------------------------------------------- | ------- | --------- | ------------------- | ----------- | ---------- | ---- | ---------------------- | --------------------------------- |
| **Kodi**                | [xbmc/xbmc](https://github.com/xbmc/xbmc)                                     | GPL-2.0 | ✅ Native | 1000s Python addons | ✅ (addon)  | ✅         | ✅   | ✅ SMB/NFS/UPnP/WebDAV | Torrent/Debrid/IPTV/Plex/Jellyfin |
| **Jellyfin Android TV** | [jellyfin/jellyfin-androidtv](https://github.com/jellyfin/jellyfin-androidtv) | GPL-2.0 | ✅ Native | Server plugins      | ✅ (plugin) | ✅ MPV     | ✅   | ✅ (via server)        | Via Jellyfin server               |

## MEDIA PLAYERS

| App                    | GitHub                                                                    | License    | ATV         | Subs           | Trakt | Ext Player | Protocols               |
| ---------------------- | ------------------------------------------------------------------------- | ---------- | ----------- | -------------- | ----- | ---------- | ----------------------- |
| **VLC for Android TV** | [videolan/vlc](https://github.com/videolan/vlc)                           | LGPL-2.1   | ✅ Native   | ✅ All formats | ❌    | No         | SMB/NFS/UPnP/HTTP/DLNA  |
| **Nova Video Player**  | [nova-video-player/aos-AVP](https://github.com/nova-video-player/aos-AVP) | GPL-3.0    | ✅ Native   | ✅             | ✅    | No         | SMB/NFS/UPnP/WebDAV/FTP |
| **Just Player**        | [moneytoo/Player](https://github.com/moneytoo/Player)                     | Unlicense  | ⚠️ Sideload | ✅             | ❌    | No         | File picker             |
| **Next Player**        | [anilbeesetti/nextplayer](https://github.com/anilbeesetti/nextplayer)     | Apache-2.0 | ⚠️ Sideload | ✅             | ❌    | No         | File picker/DASH/HLS    |

## DEBRID-FOCUSED

| App           | GitHub                                                                                      | License    | ATV         | Debrid Services                                   | Features                                                                                       |
| ------------- | ------------------------------------------------------------------------------------------- | ---------- | ----------- | ------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Debrify**   | [varunsalian/debrify](https://github.com/varunsalian/debrify)                               | Custom     | ✅ TV mode  | Real-Debrid, TorBox, PikPak                       | Stremio addons, built-in libmpv player, download queue, Jackett/Prowlarr plugins, channel mode |
| **Flixorent** | [Hashaleen420/Flixorent](https://github.com/Hashaleen420/Flixorent)                         | Apache-2.0 | ✅ TV-opt   | Real-Debrid, AllDebrid, Premiumize (BETA), TorBox | Built-in Torrentio (zero config), hybrid P2P/Debrid, auto-rank 4K→1080p→720p, Chromecast       |
| **Unchained** | [LivingWithHippos/unchained-android](https://github.com/LivingWithHippos/unchained-android) | GPL-3.0    | ⚠️ Sideload | Real-Debrid                                       | Torrent/magnet, Jackett/Prowlarr search, external player, F-Droid, mature (since 2020)         |

## YOUTUBE (Ad-Free)

| App           | GitHub                                                        | License | ATV         | Features                                                       |
| ------------- | ------------------------------------------------------------- | ------- | ----------- | -------------------------------------------------------------- |
| **SmartTube** | [yuliskov/SmartTube](https://github.com/yuliskov/SmartTube)   | MIT     | ✅ Native   | 4K/HDR, SponsorBlock, no ads, return dislikes, background play |
| **Clipious**  | [lamarios/clipious](https://github.com/lamarios/clipious)     | OSS     | ✅ Native   | Invidious client, SponsorBlock+DeArrow, audio-only, downloads  |
| **SkyTube**   | [SkyTubeTeam/SkyTube](https://github.com/SkyTubeTeam/SkyTube) | GPL-3.0 | ⚠️ Sideload | No account needed, no tracking, blocklist, OPML                |

## IPTV

| App             | GitHub                                                                  | License    | ATV       | Features                                                                 |
| --------------- | ----------------------------------------------------------------------- | ---------- | --------- | ------------------------------------------------------------------------ |
| **OwnTV**       | [ahXN00/OwnTV](https://github.com/ahXN00/OwnTV)                         | GPL-3.0    | ✅ Native | Dual engine (libmpv movies + ExoPlayer live), Xtream+M3U, fast switching |
| **Strix**       | [isnow-git/strix](https://github.com/isnow-git/strix)                   | Apache-2.0 | ✅ Native | Low-memory, budget TV focus, Compose for TV                              |
| **DangoPlayer** | [brunochanrio/DangoPlayer](https://github.com/brunochanrio/DangoPlayer) | MIT        | ✅ Native | IPTV (M3U/PLS), DRM, PiP, Google Live Channels integration               |
| **Fermata**     | [AndreyPavlenko/Fermata](https://github.com/AndreyPavlenko/Fermata)     | OSS        | ✅ Native | IPTV addon+EPG, YouTube+SponsorBlock, network folders, pluggable engines |

## TWITCH

| App               | GitHub                                                        | License  | ATV             | Features                                              |
| ----------------- | ------------------------------------------------------------- | -------- | --------------- | ----------------------------------------------------- |
| **S0undTV**       | [S0und/S0undTV](https://github.com/S0und/S0undTV)             | OSS      | ✅ Native       | Ad-free, chat, BTTV/FFZ/7TV emotes, VOD               |
| **SmartTwitchTV** | [fgl27/SmartTwitchTV](https://github.com/fgl27/SmartTwitchTV) | OSS      | ✅ Native       | Web-based, Google Play available                      |
| **ThystTV**       | [tzii/ThystTV](https://github.com/tzii/ThystTV)               | AGPL-3.0 | ✅ Large-screen | Floating chat overlay, watch history stats, Xtra fork |

## ANIME

| App            | GitHub                                                            | License    | ATV           | Features                                                          |
| -------------- | ----------------------------------------------------------------- | ---------- | ------------- | ----------------------------------------------------------------- |
| **Aniyomi**    | [aniyomiorg/aniyomi](https://github.com/aniyomiorg/aniyomi)       | Apache-2.0 | ⚠️ Sideload   | Extensions, MAL/Anilist, MPV/VLC, video+manga                     |
| **Miru**       | [miru-project/miru-app](https://github.com/miru-project/miru-app) | AGPL-3.0   | ⚠️ Sideload   | JS extensions, video/comics/novels, v2+ ATV                       |
| **Hikari**     | [Hflott/hikari_app](https://github.com/Hflott/hikari_app)         | GPL-3.0    | ✅ Native     | HAP addon protocol, AniList sync, torrent streaming, batch series |
| **OpenStream** | [Ivorisnoob/OpenStream](https://github.com/Ivorisnoob/OpenStream) | MIT        | ✅ ATV+Mobile | Material 3, TMDB metadata, HLS streaming                          |

## TRACKING

| App                   | GitHub                                                        | License  | ATV       | Services                                              |
| --------------------- | ------------------------------------------------------------- | -------- | --------- | ----------------------------------------------------- |
| **NyanTV**            | [NyanTV/NyanTV](https://github.com/NyanTV/NyanTV)             | AGPL-3.0 | ✅ Native | AniList + MyAnimeList + Simkl. Purpose-built for ATV. |
| **Trakt for Android** | [trakt/trakt-android](https://github.com/trakt/trakt-android) | GPL-3.0  | ✅ Native | Official Trakt client for Android/ATV                 |
