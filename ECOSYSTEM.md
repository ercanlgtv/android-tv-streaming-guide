# Ecosystem Map

```
                    DEBRID SERVICES
          (Real-Debrid / AllDebrid / Premiumize / TorBox)
                     │
        ┌────────────┼────────────┬────────────┐
        ▼            ▼            ▼            ▼
   DEBRID TOOLS   SCRAPERS    AUTOMATION   TORRENT NATIVE
   RDTClient     Torrentio    Riven        WebTorrent
   Zurg (WebDAV) Comet        (FUSE VFS)   Fluxstream
   DMM           MediaFusion  Seerr        GoStream
   StremThru     AIOStreams   Sonarr/Radar Stream Server
        │            │            │            │
        └────────────┴────────────┴────────────┘
                         │
                   MEDIA SERVERS
           Jellyfin (FOSS) · Plex (ref) · Emby
                         │
                         ▼
              ANDROID TV FRONTENDS
   ┌──────────────────┬──────────────────┐
   │  All-in-One     │  Single-Service  │
   │  NuvioTV        │  Jellyfin ATV    │
   │  ARVIO          │  SmartTube (YT)  │
   │  Kodi           │  Sozo (CS)       │
   │  CloudStream 3  │  VLC (local)     │
   │  MediaStorm     │  OwnTV (IPTV)    │
   │  Flixorent      │  Nova (local)    │
   └──────────────────┴──────────────────┘
```

## Integration Notes

- **CloudStream 3** can run Stremio addons via **StremioX/StremioC** plugin (in
  phisher repo)
- **Kodi** can run Stremio addons via **Stremio2Kodi** bridge
- **Syncler** can run Stremio addons via **Providra** bridge
- **Riven** mounts FUSE VFS that Jellyfin can scan as library = "request →
  appear" pipeline
- **Zurg + rclone → Jellyfin** = classic debrid mount stack
- **Comet + StremThru** = unified debrid API supporting 9 providers
- **ElfHosted** offers managed hosting for Comet, MediaFusion, Riven, MediaStorm

## Core Projects

| Layer          | Project       | URL                                                                                                   |
| -------------- | ------------- | ----------------------------------------------------------------------------------------------------- |
| Debrid         | Real-Debrid   | https://real-debrid.com                                                                               |
| Debrid         | AllDebrid     | https://alldebrid.com                                                                                 |
| Debrid         | Premiumize    | https://premiumize.me                                                                                 |
| Debrid         | TorBox        | https://torbox.app                                                                                    |
| Debrid tool    | RDTClient     | [rogerfar/rdt-client](https://github.com/rogerfar/rdt-client)                                         |
| Debrid tool    | Zurg          | [debridmediamanager/zurg](https://github.com/debridmediamanager/zurg)                                 |
| Debrid tool    | DMM           | [debridmediamanager/debrid-media-manager](https://github.com/debridmediamanager/debrid-media-manager) |
| Debrid tool    | StremThru     | [MunifTanjim/stremthru](https://github.com/MunifTanjim/stremthru)                                     |
| Scraper        | Torrentio     | https://torrentio.strem.fun                                                                           |
| Scraper        | Comet         | [g0ldyy/comet](https://github.com/g0ldyy/comet)                                                       |
| Scraper        | MediaFusion   | [mhdzumair/MediaFusion](https://github.com/mhdzumair/MediaFusion)                                     |
| Scraper        | AIOStreams    | [Viren070/AIOStreams](https://github.com/Viren070/AIOStreams)                                         |
| Scraper        | Magnetio      | [peterdsp/Magnetio](https://github.com/peterdsp/Magnetio)                                             |
| Automation     | Riven         | [rivenmedia/riven](https://github.com/rivenmedia/riven)                                               |
| Automation     | Seerr         | https://seerr.dev                                                                                     |
| Media server   | Jellyfin      | [jellyfin/jellyfin](https://github.com/jellyfin/jellyfin)                                             |
| Torrent native | WebTorrent    | [webtorrent/webtorrent](https://github.com/webtorrent/webtorrent)                                     |
| Torrent native | Fluxstream    | https://fluxstream.app                                                                                |
| Torrent native | Stream Server | [perpetus/stream-server](https://github.com/perpetus/stream-server)                                   |
| Torrent native | GoStream      | [lorenzopino/gostream](https://github.com/lorenzopino/gostream)                                       |
| Torrent native | TorrServer    | [YouROK/TorrServer](https://github.com/YouROK/TorrServer)                                             |
| Hosting        | ElfHosted     | https://elfhosted.com                                                                                 |
