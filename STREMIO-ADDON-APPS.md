# Apps That Support Stremio Addons

## NATIVE (Full Stremio Addon API)

| App                         | GitHub                                                              | Website                        | Android TV | Type       | Features                                                                                                                                                |
| --------------------------- | ------------------------------------------------------------------- | ------------------------------ | ---------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **NuvioTV**                 | [NuvioMedia/NuvioTV](https://github.com/NuvioMedia/NuvioTV)         | [nuvio.tv](https://nuvio.tv)   | ✅ Native  | GPL-3.0    | Stremio addon manfiest URLs, profiles, cross-device sync, MPV player, Trakt, debrid                                                                     |
| **ARVIO**                   | [ProdigyV21/ARVIO](https://github.com/ProdigyV21/ARVIO)             | [arvio.tv](https://arvio.tv)   | ✅ Native  | Apache-2.0 | Unifies Jellyfin + Plex + Emby **+ Stremio addons** + IPTV + Trakt in one UI                                                                            |
| **MediaStorm** (prev STRMR) | [godver3/mediastorm](https://github.com/godver3/mediastorm)         | [strmr.app](https://strmr.app) | ✅ Native  | OSS        | Stremio addon bundles, debrid, Usenet, Docker self-hosted, Android TV APK                                                                               |
| **DodoStream**              | [DodoraApp/DodoStream](https://github.com/DodoraApp/DodoStream)     | —                              | ✅ Native  | GPL-3.0    | Stremio addons, privacy-focused, React Native                                                                                                           |
| **Lumera**                  | [LumeraD3v/Lumera](https://github.com/LumeraD3v/Lumera)             | —                              | ✅ Native  | GPL-3.0    | Stremio account import, IntroDb skip intro, adaptive HLS/DASH, subtitle customization, speed control, source switching mid-playback                     |
| **Nexio**                   | [johnneerdael/nexio](https://github.com/johnneerdael/nexio)         | —                              | ✅ Native  | GPL-3.0    | Stremio addons, companion web portal, debrid-aware, multi-tracker watch state, Downloader install codes                                                 |
| **Debrify**                 | [varunsalian/debrify](https://github.com/varunsalian/debrify)       | —                              | ✅ TV mode | Custom     | Stremio addons **+** debrid manager (RD/TorBox/PikPak) + built-in libmpv player + download queue + Jackett/Prowlarr plugins                             |
| **NuvioMobile**             | [NuvioMedia/NuvioMobile](https://github.com/NuvioMedia/NuvioMobile) | —                              | ✅ Yes     | GPL-3.0    | Companion to NuvioTV, Stremio addons, has **open feature request for CloudStream plugins** [#980](https://github.com/NuvioMedia/NuvioMobile/issues/980) |

## BRIDGE (Run Stremio Addons Inside Another App)

| App         | Bridge       | GitHub                                                                                  | How it works                                                                                                                                               | Android TV            |
| ----------- | ------------ | --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| **Kodi**    | Stremio2Kodi | [VSeryi/plugin.video.stremio2kodi](https://github.com/VSeryi/plugin.video.stremio2kodi) | Kodi addon that wraps Stremio addon API — paste manifest URL, browse in Kodi UI, HDR/DV/IMAX detection, auto-play, TMDbHelper, parallel multi-addon search | ✅ Via Kodi           |
| **Syncler** | Providra     | [dtankdempsey2/Providra](https://github.com/dtankdempsey2/Providra)                     | Local Android server that converts Stremio addon response → Syncler vendor package format. Also supports Nuvio plugins                                     | ✅ Native (both apps) |
| **Chillio** | ChilliBridge | [elfhosted/chillibridge](https://github.com/elfhosted/chillibridge)                     | Server translates Stremio addon → ChillLink protocol for Chillio player. Can proxy through MediaFlow                                                       | ❌ (Apple only)       |

## PARTIAL / UNVERIFIED

| App              | GitHub                                                                    | Notes                                                                                                         |
| ---------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **PluginStream** | [PluginStream/pluginstream](https://github.com/PluginStream/pluginstream) | Listed under stremio-alternative topic, likely has plugin/addon architecture but Stremio compat not confirmed |
| **cove**         | [coveninja/cove](https://github.com/coveninja/cove)                       | MIT, cross-platform, Stremio addon-inspired, early stage, sideload on ATV                                     |
| **StreamVault**  | [Rcap2021/StreamVault](https://github.com/Rcap2021/StreamVault)           | Android streaming app, Stremio-like UI, unverified addon compatibility                                        |
| **deep-purple**  | [manuel09/deep-purple](https://github.com/manuel09/deep-purple)           | Stremio-like catalog browser for Android TV, experimental                                                     |
