# MiniArena Resource Pack

Tiered TNT textures for the MiniArena Minecraft plugin (Paper 1.21.6).

## Direct download URL

Use this in `server.properties` / the host panel as the resource pack URL:

```
https://raw.githubusercontent.com/ragyashraf/resource-pack/main/MiniArena-ResourcePack.zip
```

SHA-1 of the zip:

```
a61e72adf5972b743978a67569a594e7d2081b5d
```

Set both values in the server properties (`resource-pack` and
`resource-pack-sha1`), then restart. Players are prompted to download the pack
when they join.

## What it contains

Five TNT tiers, each retextured so the item is distinguishable in the hotbar:

| Tier | Model data | Colour |
|------|-----------|--------|
| Normal TNT | 2 | classic red |
| Strong TNT | 3 | orange |
| Super TNT | 4 | deep red |
| Mega TNT | 5 | purple |
| Ultra TNT | 6 | dark violet |

Textures are keyed on `custom_model_data` via `assets/minecraft/items/tnt.json`
using the 1.21.4+ item model format.

## Note on placed blocks

Custom model data applies to the **item**, not to placed blocks. Minecraft
provides no way for a plugin or pack to give a placed vanilla TNT block a
per-tier texture, so a built tower renders as ordinary TNT. The tier is still
visible in the hotbar, in the item name, and in blast power.

## Repository layout

- `MiniArena-ResourcePack.zip` — the packaged pack, ready to serve
- `resourcepack/` — unpacked sources, for editing

After editing anything under `resourcepack/`, re-zip its **contents** (so
`pack.mcmeta` sits at the zip root, not inside a folder) and update the SHA-1
in the server properties.
