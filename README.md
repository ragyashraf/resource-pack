# Noctis Nova Resource Pack

Textures for the MiniArena plugin: tiered TNT blocks, and the casino card,
chip, and roulette artwork.

## Contents

| Group | Files | Notes |
| --- | --- | --- |
| TNT tiers | 5 block models | normal / strong / super / mega / ultra |
| Playing cards | 52 + back | full deck, corner rank and suit pip |
| Casino chips | 5 + locked | white 100, red 500, green 1k, black 5k, purple 25k |
| Roulette pockets | 3 | red / black / green |
| Buttons | 2 | Higher / Lower arrows |

All casino textures are 16x16 and original work. See `TEXTURE_CREDITS.txt`
for the TNT texture attributions.

## Serving the pack

    resource-pack=https://raw.githubusercontent.com/ragyashraf/resource-pack/main/MiniArena-ResourcePack.zip
    resource-pack-sha1=97430ddeaad1d20e0b7adf2c4e359b2e38d44ba5

Commit-pinned jsDelivr, if raw.githubusercontent is unreliable:

    resource-pack=https://cdn.jsdelivr.net/gh/ragyashraf/resource-pack@main/MiniArena-ResourcePack.zip
    resource-pack-sha1=97430ddeaad1d20e0b7adf2c4e359b2e38d44ba5

Alternatively the plugin can prompt for the pack itself, which shows a custom
message and only asks once the player has logged in. In `config.yml`:

```yaml
resource-pack:
  url: 'https://raw.githubusercontent.com/ragyashraf/resource-pack/main/MiniArena-ResourcePack.zip'
  sha1: '97430ddeaad1d20e0b7adf2c4e359b2e38d44ba5'
  required: false
```

`required` can stay `false`: every custom item has a sensible fallback
material, so the casino is still playable without the pack, just less legible.

## Updating

The SHA-1 above must match `MiniArena-ResourcePack.zip` exactly. Clients cache
packs by hash, so a changed zip with a stale hash is rejected and players see
no textures at all. After rebuilding the zip:

```
# Windows
certutil -hashfile MiniArena-ResourcePack.zip SHA1
# Linux / macOS
sha1sum MiniArena-ResourcePack.zip
```

Then update the hash in this README and in the plugin's `config.yml`.

Rebuild the zip from the `resourcepack/` folder with `pack.mcmeta` at the
archive root - not nested inside a parent directory, or the client rejects it.
