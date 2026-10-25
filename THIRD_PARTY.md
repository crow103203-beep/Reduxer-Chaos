# Third-party dependencies and publication review

Reviewed on 2026-10-25. This is an inventory and record of evidence, not a new license grant.

## Libraries omitted from the source archive

| Library | Evidence | Publication decision |
| --- | --- | --- |
| Upgrader 1.2.1 | Bundled `META-INF/neoforge.mods.toml`: All Rights Reserved; [upstream project](https://modrinth.com/mod/UQgc9Wcb) also labels ARR | Do not host the JAR; obtain the pinned build from upstream. |
| ProtoManly's Weather 0.17.16-alpha | Bundled metadata: All Rights Reserved; [upstream page](https://modrinth.com/mod/protomanlys-weather) permits freely available packs but says not to redistribute JAR files | Do not host the JAR; preserve the Modrinth download reference. Its nested Veil dependency is also not copied into this repository. |
| TerraBlender 4.1.0.8 | Bundled metadata: LGPLv3; [upstream repository](https://github.com/Glitchfiend/TerraBlender) lists LGPL-3.0 | Omitted with the other local build libraries; obtain from upstream. |

The original source ZIP contained all three binaries in `libs/`. The published source ZIP excludes the entire `libs/` directory and includes instructions for obtaining these dependencies. Original project source files are preserved byte-for-byte.

## Custom project and artwork

The supplied addon metadata declares MIT, but the source archive contains no LICENSE file. No repository-wide license has been added because the rights and intended scope were not confirmed. Existing addon metadata has not been rewritten. The supplied Reduxer artwork is included as project artwork; no additional reuse license is granted for it.

## Modpack format

The supplied `.mrpack` has two entries: `modrinth.index.json` and the custom addon under `overrides/mods/`. The embedded addon is byte-identical to the separately supplied JAR. It contains 51 class files, all under `ru/upgraderchaos/`, and no nested dependency JARs. The manifest provides SHA-1 and SHA-512 hashes and Modrinth CDN URLs for 31 upstream files.

Those third-party files are downloaded from the original hosting service; they are not republished here. The inventory below does not imply that their licenses are identical or that users may rehost them. Consult each author's current terms before redistribution. Other third-party mod licenses were not individually certified for binary redistribution, which this publication does not perform.

## Pinned upstream files

| File | Upstream project |
| --- | --- |
| `pmweather-1.21.1-0.17.16-alpha.jar` | [Modrinth TfCsmTLI](https://modrinth.com/mod/TfCsmTLI) |
| `upgrader-neoforge-1.2.1+1.21.1.jar` | [Modrinth UQgc9Wcb](https://modrinth.com/mod/UQgc9Wcb) |
| `mowziesmobs-1.21.1-1.8.2.jar` | [Modrinth BFbX9xcm](https://modrinth.com/mod/BFbX9xcm) |
| `naturalist-2.0.7-neoforge-1.21.1.jar` | [Modrinth F8BQNPWX](https://modrinth.com/mod/F8BQNPWX) |
| `CreeperOverhaul-neoforge-1.21.1-4.0.6.jar` | [Modrinth MI1LWe93](https://modrinth.com/mod/MI1LWe93) |
| `crittersandcompanions-neoforge-1.21.1-2.7.0.jar` | [Modrinth Yd4wb5wZ](https://modrinth.com/mod/Yd4wb5wZ) |
| `legendary_monsters-2.2.4 MC 1.21.1.jar` | [Modrinth 9d9Bkqva](https://modrinth.com/mod/9d9Bkqva) |
| `endermanoverhaul-neoforge-1.21.1-2.0.3.jar` | [Modrinth Lq6ojcWv](https://modrinth.com/mod/Lq6ojcWv) |
| `zombieawareness-neoforge-1.21.0-1.13.2.jar` | [Modrinth mMTOWOaA](https://modrinth.com/mod/mMTOWOaA) |
| `sodium-neoforge-0.8.13+mc1.21.1.jar` | [Modrinth AANobbMI](https://modrinth.com/mod/AANobbMI) |
| `ferritecore-7.0.3-neoforge.jar` | [Modrinth uXXizFIs](https://modrinth.com/mod/uXXizFIs) |
| `modernfix-neoforge-5.27.27+mc1.21.1.jar` | [Modrinth nmDcB62a](https://modrinth.com/mod/nmDcB62a) |
| `jei-1.21.1-neoforge-19.64.0.455.jar` | [Modrinth u6dRKJwZ](https://modrinth.com/mod/u6dRKJwZ) |
| `Jade-1.21.1-NeoForge-15.10.6.jar` | [Modrinth nvQzSEkH](https://modrinth.com/mod/nvQzSEkH) |
| `appleskin-neoforge-mc1.21-3.0.9.jar` | [Modrinth EsAfCjCV](https://modrinth.com/mod/EsAfCjCV) |
| `MouseTweaks-neoforge-mc1.21-2.26.1.jar` | [Modrinth aC3cM3Vq](https://modrinth.com/mod/aC3cM3Vq) |
| `AmbientSounds_NEOFORGE_v6.3.11_mc1.21.1.jar` | [Modrinth fM515JnW](https://modrinth.com/mod/fM515JnW) |
| `TerraBlender-neoforge-1.21.1-4.1.0.8.jar` | [Modrinth kkmrDlKT](https://modrinth.com/mod/kkmrDlKT) |
| `entityculling-neoforge-1.11.3-mc1.21.1.jar` | [Modrinth NNAgCjsB](https://modrinth.com/mod/NNAgCjsB) |
| `lithium-neoforge-0.15.4+mc1.21.1.jar` | [Modrinth gvQqBUqZ](https://modrinth.com/mod/gvQqBUqZ) |
| `ImmediatelyFast-NeoForge-1.6.15+1.21.1.jar` | [Modrinth 5ZwdcRci](https://modrinth.com/mod/5ZwdcRci) |
| `dynamic-fps-3.11.4+minecraft-1.21.0-neoforge.jar` | [Modrinth LQ3K71Q1](https://modrinth.com/mod/LQ3K71Q1) |
| `AI-Improvements-1.21-0.5.3.jar` | [Modrinth DSVgwcji](https://modrinth.com/mod/DSVgwcji) |
| `geckolib-neoforge-1.21.1-4.9.3.jar` | [Modrinth 8BmcQJ2H](https://modrinth.com/mod/8BmcQJ2H) |
| `resourcefulconfig-neoforge-1.21-3.0.11.jar` | [Modrinth M1953qlQ](https://modrinth.com/mod/M1953qlQ) |
| `resourcefullib-neoforge-1.21-3.0.12.jar` | [Modrinth G1hIVOrD](https://modrinth.com/mod/G1hIVOrD) |
| `architectury-13.0.11-neoforge.jar` | [Modrinth lhGA9TYQ](https://modrinth.com/mod/lhGA9TYQ) |
| `yet_another_config_lib_v3-3.8.2+1.21.1-neoforge.jar` | [Modrinth 1eAoo2KR](https://modrinth.com/mod/1eAoo2KR) |
| `coroutil-neoforge-1.21.0-1.3.8.jar` | [Modrinth rLLJ1OZM](https://modrinth.com/mod/rLLJ1OZM) |
| `mezz_config-1.21.1-neoforge-0.6.8-standalone.jar` | [Modrinth 7tEfOcA7](https://modrinth.com/mod/7tEfOcA7) |
| `CreativeCore_NEOFORGE_v2.13.51_mc1.21.1.jar` | [Modrinth OsZiaDHq](https://modrinth.com/mod/OsZiaDHq) |

## Review limits

Static pattern scanning of 3,376 files/archive entries found no matches for the configured private-key, GitHub-token, AWS-key, service-token, quoted-credential, credential-URL or Discord-webhook patterns. No actual secret values are included in this report. This cannot establish the absence of all secrets or malware. The source scripts and supplied binaries were inspected without execution. No fresh build or game test was performed, and binary/source reproducibility was not established. Upstream URLs and hashes were structurally checked; all referenced files were not downloaded again.
