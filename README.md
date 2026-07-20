# MiniArena Resource Pack

Tiered TNT textures for the MiniArena Minecraft plugin (Paper 1.21.6).

## Direct download URL

Use this in `server.properties` / the host panel as the resource pack URL:

```
https://raw.githubusercontent.com/ragyashraf/resource-pack/main/MiniArena-ResourcePack.zip
```

SHA-1 of the zip:

```
37ca328aee744a67c9c59a14234a145e3eb82828
```

Set both values in the server properties (`resource-pack` and `resource-pack-sha1`), then restart. Players are prompted to download the pack when they join.

## What it contains

Five TNT tiers via `item_model` (`miniarena:tnt_*`) plus CMD fallback:

| Tier | item_model | Design |
| ---------- | ---------- | ----------- |
| Normal TNT | miniarena:tnt_normal | Magex Barrel TNT |
| Strong TNT | miniarena:tnt_strong | TNT Rust |
| Super TNT | miniarena:tnt_super | Red TNT Barrel |
| Mega TNT | miniarena:tnt_mega | Nuclear TNT |
| Ultra TNT | miniarena:tnt_ultra | Black TNT |

## Texture credits

See `resourcepack/TEXTURE_CREDITS.txt`.

## Repository layout

* `MiniArena-ResourcePack.zip` — packaged pack
* `resourcepack/` — sources

After editing, re-zip contents (`pack.mcmeta` at zip root) and update the SHA-1 above.
