# Final Recommendations

## Best Android TV Experience

→ **ARVIO** — Purpose-built for TV (Leanback UI). Unifies Jellyfin + Plex +
Emby + Stremio addons + IPTV in one app. Free. Apache 2.0. → **NuvioTV** —
Excellent native ATV experience. Stremio addons + profiles + MPV + cross-device
sync.

## Best FOSS Project

→ **Jellyfin** ([jellyfin/jellyfin](https://github.com/jellyfin/jellyfin)) —
52.6k★. Healthiest, most active FOSS media project. Complete server + excellent
Android TV client.

## Best Plugin Ecosystem

→ **Kodi** ([xbmc/xbmc](https://github.com/xbmc/xbmc)) — Thousands of addons.
Python SDK. Stremio2Kodi bridge brings Stremio addons into Kodi.

## Best Replacement for Stremio

→ **NuvioTV** ([NuvioMedia/NuvioTV](https://github.com/NuvioMedia/NuvioTV)) —
Full Stremio addon compatibility. Free profiles (Stremio charges $39.99/yr).
Cross-device sync. MPV. Trakt. → **ARVIO** — Better if you also use
Jellyfin/Plex. Unifies everything.

## Best Replacement for CloudStream

→ **CloudStream 3**
([recloudstream/cloudstream](https://github.com/recloudstream/cloudstream)) —
Still actively maintained. No other app comes close to its `.cs3` plugin
ecosystem. Android TV performance issues acknowledged. → **Kodi + Stremio2Kodi**
([VSeryi/plugin.video.stremio2kodi](https://github.com/VSeryi/plugin.video.stremio2kodi))
— More stable on Android TV, uses Stremio addons through bridge.

## Best Lightweight Option

→ **Flixorent**
([Hashaleen420/Flixorent](https://github.com/Hashaleen420/Flixorent)) — <70MB
APK. Built-in Torrentio. No plugin configuration. Debrid + P2P. Apache 2.0.

## Best Power-User Option

→ **Kodi** — Maximum customization. Every protocol. Dolby Atmos/TrueHD
passthrough. Audio DSP. RetroPlayer. PVR/DVR. Skins. Nothing else comes close.

## Best Long-Term Maintained

→ **Jellyfin** (~400 contributors, community foundation, predictable releases,
growing adoption).

## Recommended Combos

### One App To Rule Them All

```
Install ARVIO → add Jellyfin/Plex servers + Stremio addon URLs + IPTV playlist
→ One UI for everything
```

### Stremio Replacement (Most Familiar)

```
NuvioTV (movies/TV via Stremio addons)
+ SmartTube (ad-free YouTube)
```

### Self-Hosted Power Setup

```
Jellyfin Server (media server)
  → Riven (debrid automation fills library)
  → ARVIO or Jellyfin Android TV (frontend)
  → Seerr (content requests)
```

### Budget / Low-End TV

```
Flixorent (built-in Torrentio + Real-Debrid, zero config)
+ SmartTube (YouTube)
+ OwnTV (IPTV if needed)
```

### CloudStream Replacement

```
CloudStream 3 (latest recloudstream fork)
  → add Phisher repo + StremioX plugin
OR
Kodi + Stremio2Kodi (for stability)
  → add Stremio addons of choice
```
