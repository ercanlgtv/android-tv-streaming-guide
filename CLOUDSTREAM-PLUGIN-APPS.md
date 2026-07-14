# Apps That Support CloudStream Plugins

## SUMMARY

Only **2 non-fork apps** can load native `.cs3` CloudStream plugins. No
mainstream Android TV streaming app supports them natively besides CloudStream
itself.

---

## NATIVE CS3 LOADER

| App                 | GitHub                                                                                          | Loads .cs3?                  | Android TV       | How                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------- | ---------------------------- | ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Sozo (Soplay)**   | [professorDeveloper/sozo](https://github.com/professorDeveloper/sozo)                           | ✅ Yes — uses DexClassLoader | ✅ Flutter-based | RepoManager downloads .cs3 → PluginHost loads via PathClassLoader → providers register as `cs:<name>`. ~70/73 plugins from phisher98 repo work. Advanced plugins referencing app-module classes may fail. |
| **cloudstream-web** | [mindflarevortx-maker/cloudstream-web](https://github.com/mindflarevortx-maker/cloudstream-web) | ❌ No (JS ports only)        | ❌ Web           | TypeScript reimplementation of CloudStream MainAPI. Cannot load DEX bytecode. Has JS ports of same providers. Runtime sandbox.                                                                            |

## FEATURE REQUEST (NOT IMPLEMENTED)

| App             | Issue                                                        | Status                                                                                                      |
| --------------- | ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------- |
| **NuvioMobile** | [#980](https://github.com/NuvioMedia/NuvioMobile/issues/980) | Open — requested repo.json support, GitHub raw links install, compatibility layer for existing CS providers |

## CLOUDSTREAM ITSELF (Still Active)

| Fork                          | GitHub                                                                             | Stars            |
| ----------------------------- | ---------------------------------------------------------------------------------- | ---------------- |
| **recloudstream/cloudstream** | [recloudstream/cloudstream](https://github.com/recloudstream/cloudstream)          | 10.1k★           |
| **Stormunblessed**            | [Stormunblessed/cloudstream-3](https://github.com/Stormunblessed/cloudstream-3)    | 131★             |
| **AniFOSS**                   | [AniFOSS/CloudStream-3](https://github.com/AniFOSS/CloudStream-3)                  | 85★              |
| **cloudstream3/cs3-android**  | [cloudstream3/cs3-android](https://github.com/cloudstream3/cs3-android)            | New official org |
| **Original (archived)**       | [LagradOst/CloudStream-3](https://codeberg.org/cloudstream/cloudstream) (Codeberg) | Archived 2023    |

## WHY CS PLUGIN COMPATIBILITY IS RARE

- `.cs3` files are compiled Kotlin bytecode (DEX) — require Android's
  `DexClassLoader`/`PathClassLoader`
- Tied to `com.lagradost.cloudstream3` API surface (`MainAPI`, `ExtractorApi`,
  `@CloudstreamPlugin`)
- GPL-3.0 copyleft — bundling the CloudStream runtime makes derivative work
- Android-specific (Context, OkHttp CloudflareKiller interceptors,
  RepositoryManager)

## CS PLUGIN REPOSITORIES

| Name               | URL                                                                                           | Description                                                    |
| ------------------ | --------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| **phisher98**      | [cloudstream-extensions-phisher](https://github.com/phisher98/cloudstream-extensions-phisher) | 78 providers, movies/TV/anime/live/torrent/music, 16 languages |
| **MegaRepo**       | [self-similarity/MegaRepo](https://github.com/self-similarity/MegaRepo)                       | Meta-installer — installs all known repos at once              |
| **cs3plugs**       | [justsimplyleon/cs3plugs](https://github.com/justsimplyleon/cs3plugs)                         | Curated list of working plugins                                |
| **CSX**            | [SaurabhKaperwan/CSX](https://github.com/SaurabhKaperwan/CSX)                                 | Additional provider collection                                 |
| **Official repos** | [recloudstream/cs-repos](https://github.com/recloudstream/cs-repos)                           | Official repo database                                         |

## BRIDGE — CLOUDSTREAM RUNNING THIRD-PARTY PLUGINS (Opposite Direction)

| Project                    | GitHub                                                                                          | What it does                                                                |
| -------------------------- | ----------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| **AniyomiCompatExtension** | [CranberrySoup/AniyomiCompatExtension](https://github.com/CranberrySoup/AniyomiCompatExtension) | Runs Aniyomi extensions **inside** CloudStream. Not the direction you want. |
| **StremioX / StremioC**    | In phisher98 repo                                                                               | Runs Stremio addons **inside** CloudStream                                  |
