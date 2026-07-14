# Feature Comparison

| App                  | Open Source  | Android TV  | TV Remote    | Stremio Addons          | CS Plugins     | Plugin System       | Trakt       | Sync | Ext Player     | Subs |
| -------------------- | ------------ | ----------- | ------------ | ----------------------- | -------------- | ------------------- | ----------- | ---- | -------------- | ---- |
| **NuvioTV**          | GPL-3.0      | ✅ Native   | ✅ Excellent | ✅ Native               | ❌ (requested) | Stremio addons      | ✅          | ✅   | ✅ MPV         | ✅   |
| **ARVIO**            | Apache-2.0   | ✅ Native   | ✅ Excellent | ✅ Native               | ❌             | Stremio addons      | ✅          | ✅   | ❌             | ✅   |
| **MediaStorm**       | OSS          | ✅ Native   | ✅ Good      | ✅ Native               | ❌             | Stremio addons      | ✅          | ✅   | ✅             | ✅   |
| **DodoStream**       | GPL-3.0      | ✅ Native   | ✅ Good      | ✅ Native               | ❌             | Stremio addons      | ❌          | ❌   | ❌             | ✅   |
| **Lumera**           | GPL-3.0      | ✅ Native   | ✅ Good      | ✅ Native               | ❌             | Stremio addons      | ❌          | ❌   | ❌             | ✅   |
| **Nexio**            | GPL-3.0      | ✅ Native   | ✅ Good      | ✅ Native               | ❌             | Stremio addons      | ❌          | ✅   | ❌             | ✅   |
| **Debrify**          | Custom       | ✅ TV mode  | ✅ Good      | ✅ Native               | ❌             | Jackett/Prowlarr    | ✅          | ❌   | ✅             | ✅   |
| **Kodi**             | GPL-2.0      | ✅ Native   | ✅ Excellent | ⚠️ Via bridge           | ❌             | 1000s Python addons | ✅ (addon)  | ✅   | ✅             | ✅   |
| **Jellyfin ATV**     | GPL-2.0      | ✅ Native   | ✅ Excellent | ❌                      | ❌             | Server plugins      | ✅ (plugin) | ✅   | ✅ MPV         | ✅   |
| **CloudStream 3**    | GPL-3.0      | ✅ Native   | ⚠️ Fair      | ⚠️ Via plugin           | ✅ Native      | .cs3 plugins        | ✅          | ❌   | ✅ MPV/VLC     | ✅   |
| **Sozo**             | ❓           | ✅ Flutter  | ⚠️ Fair      | ❌                      | ✅ Native      | CS plugins          | ❌          | ❌   | ❓             | ❓   |
| **Flixorent**        | Apache-2.0   | ✅ TV-opt   | ✅ Good      | ❌ (Torrentio built-in) | ❌             | No                  | ❌          | ❌   | ✅ VLC/MX      | ✅   |
| **VLC ATV**          | LGPL-2.1     | ✅ Native   | ✅ Excellent | ❌                      | ❌             | No                  | ❌          | ❌   | No (is player) | ✅   |
| **Nova Player**      | GPL-3.0      | ✅ Native   | ✅ Good      | ❌                      | ❌             | No                  | ✅          | ❌   | No             | ✅   |
| **SmartTube**        | MIT          | ✅ Native   | ✅ Excellent | ❌                      | ❌             | No                  | ❌          | ✅   | No             | ✅   |
| **Miru**             | AGPL-3.0     | ⚠️ Sideload | ⚠️ Fair      | ❌                      | ❌             | JS extensions       | ❌          | ❌   | No             | ❌   |
| **OwnTV**            | GPL-3.0      | ✅ Native   | ✅ Excellent | ❌                      | ❌             | No                  | ❌          | ❌   | No             | ❌   |
| **Stremio2Kodi**     | GPL-3.0      | ✅ Via Kodi | ✅ Kodi      | ✅ Bridge               | ❌             | Via Kodi            | ✅          | ✅   | ✅ Kodi        | ✅   |
| **Providra+Syncler** | GPL (bridge) | ✅ Native   | ✅ Good      | ✅ Bridge               | ❌             | Via Syncler         | ✅          | ✅   | ✅             | ✅   |

## Debrid Services Supported

| App               | Real-Debrid | AllDebrid   | Premiumize  | TorBox      | Debrid-Link |
| ----------------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| **NuvioTV**       | ✅          | ✅          | ✅          | ✅          | ✅          |
| **ARVIO**         | ✅          | ✅          | ✅          | ✅          | ✅          |
| **MediaStorm**    | ✅          | ✅          | ✅          | ✅          | ✅          |
| **Flixorent**     | ✅          | ✅          | ⚠️ Beta     | ✅          | ❌          |
| **Debrify**       | ✅          | ❌          | ❌          | ✅          | ❌          |
| **Unchained**     | ✅          | ❌          | ❌          | ❌          | ❌          |
| **Kodi**          | ✅ (addons) | ✅ (addons) | ✅ (addons) | ✅ (addons) | ✅ (addons) |
| **CloudStream 3** | ⚠️ Limited  | ⚠️ Limited  | ❌          | ❌          | ❌          |

## Streaming Protocols

| App              | Torrent      | IPTV            | WebDAV      | SMB         | NFS         | UPnP/DLNA | FTP         | HTTP |
| ---------------- | ------------ | --------------- | ----------- | ----------- | ----------- | --------- | ----------- | ---- |
| **Kodi**         | ✅ (addons)  | ✅ (PVR)        | ✅          | ✅          | ✅          | ✅        | ✅          | ✅   |
| **Jellyfin ATV** | ❌           | ✅ (server)     | ✅ (server) | ✅ (server) | ✅ (server) | ❌        | ✅ (server) | ✅   |
| **VLC ATV**      | ❌           | ✅ (playlist)   | ✅          | ✅          | ❌          | ✅        | ❌          | ✅   |
| **Nova Player**  | ❌           | ❌              | ✅          | ✅          | ✅          | ✅        | ✅          | ❌   |
| **NuvioTV**      | ✅ (Stremio) | ❌              | ❌          | ❌          | ❌          | ❌        | ❌          | ❌   |
| **ARVIO**        | ✅ (Stremio) | ✅              | ❌          | ❌          | ❌          | ❌        | ❌          | ❌   |
| **OwnTV**        | ❌           | ✅ (M3U/Xtream) | ❌          | ❌          | ❌          | ❌        | ❌          | ❌   |
| **LitPlayer**    | ❌           | ❌              | ✅          | ✅          | ❌          | ✅        | ✅          | ❌   |
| **Fermata**      | ❌           | ✅ (addon)      | ❌          | ✅          | ❌          | ❌        | ✅          | ✅   |
