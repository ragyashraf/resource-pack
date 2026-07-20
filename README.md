# MiniArena Resource Pack

Tiered TNT textures for the MiniArena Minecraft plugin (Paper 1.21.6).

## Direct download URL

Use this in `server.properties` / the host panel as the resource pack URL:

```
https://raw.githubusercontent.com/ragyashraf/resource-pack/main/MiniArena-ResourcePack.zip
```

SHA-1 of the zip:

```
f13ab0f6a46a90fe89a3405488ff047ae290be4e
```

Set both values in the server properties (`resource-pack` and `resource-pack-sha1`), then restart. Players are prompted to download the pack when they join.

## What it contains

Five TNT tiers, each with a distinct design so the item (and placed ItemDisplay overlay) is distinguishable:

| Tier | Model data | Design |
| ---------- | ---------- | ----------- |
| Normal TNT | 2 | Magex Barrel TNT |
| Strong TNT | 3 | TNT Rust |
| Super TNT | 4 | Red TNT Barrel |
| Mega TNT | 5 | Nuclear TNT |
| Ultra TNT | 6 | Black TNT |

Textures are keyed on `custom_model_data` via `assets/minecraft/items/tnt.json` using the 1.21.4+ item model format.

Vanilla `minecraft:block/tnt` is emptied so the plugin overlays show without z-fighting.

## Texture credits

See `resourcepack/TEXTURE_CREDITS.txt`. Source packs from Modrinth; original authors retain their rights.

## Repository layout

* `MiniArena-ResourcePack.zip` — the packaged pack, ready to serve
* `resourcepack/` — unpacked sources, for editing

After editing anything under `resourcepack/`, re-zip its **contents** (so `pack.mcmeta` sits at the zip root, not inside a folder) and update the SHA-1 in this README and in server properties.
