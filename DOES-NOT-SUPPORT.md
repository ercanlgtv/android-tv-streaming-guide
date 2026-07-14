# Popular Apps That Do NOT Support Stremio Addons or CloudStream Plugins

## No Stremio Addon Support

| App              | Type               | Alternative system                     | Notes                                               |
| ---------------- | ------------------ | -------------------------------------- | --------------------------------------------------- |
| **CinemaHD**     | Streaming          | Own scrapers                           | Effectively shut down early 2026                    |
| **NovaTV**       | Streaming          | Own scrapers                           | Closed-source                                       |
| **BeeTV**        | Streaming          | Own scrapers                           | Closed-source                                       |
| **CyberFlix**    | Streaming          | Own scrapers                           | Defunct                                             |
| **FilmPlus**     | Streaming          | Own scrapers                           | Closed-source                                       |
| **TeaTV**        | Streaming          | Own scrapers                           | Closed-source                                       |
| **PopcornTime**  | Torrent streaming  | Built-in torrent scraper only          | Desktop rewrite active, no ATV                      |
| **HDO Box**      | Streaming          | Own sources                            | Closed-source                                       |
| **OnStream**     | Streaming          | Own sources                            | Declining quality                                   |
| **Weyd**         | Streaming          | Own provider package system            | Proprietary, paid                                   |
| **Plex**         | Media server       | Own plugin/channel system (deprecated) | Proprietary                                         |
| **Jellyfin**     | Media server       | Jellyfin plugins                       | Bridges exist TO Jellyfin from Stremio, not reverse |
| **Emby**         | Media server       | Emby plugins                           | Proprietary                                         |
| **Infuse**       | Video player       | Plex/Jellyfin/Emby + local             | No addon system                                     |
| **VidHub**       | Video player       | Cloud drives                           | No addon system                                     |
| **Flud**         | Torrent downloader | None                                   | Downloader only                                     |
| **LibreTorrent** | Torrent downloader | None                                   | Downloader only                                     |

## No CloudStream Plugin Support

| App                            | Type            | Why                                                     |
| ------------------------------ | --------------- | ------------------------------------------------------- |
| **Miru**                       | Anime streaming | Uses own JS extension API, cannot load `.cs3` DEX files |
| **Aniyomi**                    | Anime streaming | Uses APK-based extensions (Tachiyomi-style), not `.cs3` |
| **Stremio**                    | Streaming       | Uses JSON addon manifest system, not `.cs3`             |
| **Syncler**                    | Streaming       | Proprietary vendor package format                       |
| **Kodi**                       | Media center    | Python addons, no DEX classloader                       |
| **BeeTV / CinemaHD / HDO Box** | Streaming       | Closed-source, no plugin system at all                  |
| **DangoPlayer**                | IPTV player     | IPTV/video player only, no plugin system                |
| **Filmly / MediaBox**          | Streaming       | Proprietary, no public plugin API                       |
