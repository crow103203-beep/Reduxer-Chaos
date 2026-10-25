# Reduxer-Chaos

![Reduxer-Chaos artwork](reduxer-avatar.webp)

**Turn an item into a catastrophe.** A Minecraft Java 1.21.1 modpack with the custom **Upgrader: Chaos** addon (`upgrader_chaos`, version 1.3.1), built for NeoForge 21.1.264.

The original pack name is **Сжатый Хаос** (Compressed Chaos). Reduxer-Chaos is the repository name; the supplied game files keep their original names and metadata.

## Download and install

- **Full modpack:** [upgrader-chaos-pack-1.3.1.mrpack](upgrader-chaos-pack-1.3.1.mrpack). Open the file on GitHub and use **Download raw file**, then import it into a launcher that supports Modrinth packs, such as Prism Launcher or the Modrinth App.
- **Addon only:** [upgrader-chaos-neoforge-1.21.1-1.3.1.jar](upgrader-chaos-neoforge-1.21.1-1.3.1.jar). Download the raw file and place it in a compatible instance's `mods` folder. It is not the complete modpack.
- **Source:** [upgrader-chaos-source-1.3.1.zip](upgrader-chaos-source-1.3.1.zip). This reviewed source archive excludes the third-party binaries from the original upload.
- [Русское описание](README.ru.md)

Use **Java 21**, **Minecraft Java 1.21.1** and **NeoForge 21.1.264**. The supplied pack description recommends allocating **6–8 GB RAM**. Start in a new world or back up an existing world: some events and storms destroy terrain and buildings.

The modpack contains 31 upstream download references and the custom addon. Its launcher downloads third-party mods from Modrinth; their JAR files are not hosted in this repository.

For a manual addon installation, install **Upgrader 1.2.1** and **TerraBlender 4.1.0.8** for NeoForge 1.21.1. **ProtoManly's Weather 0.17.16-alpha** is optional for the addon, but is included by reference in the full pack and enables its weather integration. Follow each upstream project's dependency requirements. The supplied PMWeather build bundles Veil 4.2.1.

## Gameplay

Put an item or stack into an upgrader to consume it and trigger a random phenomenon. The interface shows the probabilities before compression. Item value influences which events are likely.

| Upgrader | Theme | Examples |
| --- | --- | --- |
| Green | Nature | Weather, time and effects |
| Blue | Mind | Sounds, vision and hallucinations |
| Yellow | Creatures and belongings | Mobs and inventory changes |
| Red | Body and terrain | Organ loss and changes to the world |
| Purple | Storms and mysteries | Tornadoes, supercells and unusual events |

You receive the green upgrader on your first world login. Progress through the workshop in each upgrader to make the next tier. Explore the purple **Chaos Lands** biome for trees and ores, and use the Chaos Compass to help find it.

The addon defines 90 phenomena, including storms, organ effects, sound distortion, hallucinations, mob invasions and gravity changes. Mob integrations depend on the installed mods.

- **I:** open the phenomenon index.
- **Integrity Amulet:** protects against the next organ loss.
- **`/chaos list`** and **`/chaos organs`:** inspect phenomena and organ state.

The full pack references Mowzie's Mobs, Naturalist, Creeper Overhaul, Legendary Monsters, Enderman Overhaul, Critters and Companions, JEI, Jade and AppleSkin, alongside performance mods and dependencies. See [THIRD_PARTY.md](THIRD_PARTY.md) for the pinned mod list and upstream links.

## Build the addon from source

1. Extract `upgrader-chaos-source-1.3.1.zip` and open its `upgrader-chaos` directory.
2. Install JDK 21 and a Gradle version compatible with NeoForge ModDevGradle 2.0.148. The supplied project does **not** include a Gradle wrapper.
3. Create `libs/` and obtain these exact NeoForge 1.21.1 builds from their upstream projects:
   - `upgrader-neoforge-1.2.1+1.21.1.jar`
   - `pmweather-1.21.1-0.17.16-alpha.jar`
   - `TerraBlender-neoforge-1.21.1-4.1.0.8.jar`
4. Run `gradle build` from that directory. The addon is written to `build/libs/`.

All three libraries are compile-time dependencies in the supplied build, even though PMWeather is optional at runtime. Local dependency binaries and game instances are ignored by `.gitignore`.

`pack/make-pack.ps1` is the original packaging helper. It requires an external mod index, downloaded mods and the built addon. Its plain-folder output copies third-party binaries and must not be uploaded here; the `.mrpack` form uses upstream download references. The helper replaces staging/output directories, so use a dedicated output directory.

## Rights and verification

No repository-wide license has been added. The supplied addon metadata declares `MIT`, but no license text or confirmation of rights accompanied the source archive. That existing metadata has been preserved; it does not grant a license over this entire modpack, artwork or third-party mods. A maintainer must resolve the project license before describing the complete project as open source.

Upgrader and ProtoManly's Weather declare **All Rights Reserved**. PMWeather's project page allows freely available modpacks but prohibits redistributing its JAR. TerraBlender declares **LGPL-3.0**. The source archive excludes all three library JARs. Third-party mods retain their own licenses and credits.

Publication preparation included a static secret-pattern scan and archive inspection. No matching credential patterns were found. The addon JAR contains only `ru/upgraderchaos/` class files and no nested JARs; the `.mrpack` embeds only that same addon and uses Modrinth CDN links for the remaining mods. This is not a malware certification. The supplied binaries were not rebuilt or play-tested during publication preparation.

Not an official Minecraft product. Not approved by or associated with Mojang or Microsoft.
