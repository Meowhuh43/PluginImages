# Meowhuh plugin images

Shared PNG assets for Meowhuh's Rust server plugins. Each plugin has its own folder.

```
CasinoSystem/Images/*.png
AnotherPlugin/Images/*.png
```

Use direct raw image URLs in plugin image settings. Keep existing paths stable when adding images for another plugin.

Raw URL prefix: `https://raw.githubusercontent.com/Meowhuh43/PluginImages/main/`

Example: `https://raw.githubusercontent.com/Meowhuh43/PluginImages/main/CasinoSystem/Images/Red-Chip.png`

## CasinoSystem local images

Copy the `CasinoSystem/Images` folder into the Carbon data directory, keeping the same relative path. Set `"Enable Offline Image Mode": true` in CasinoSystem's configuration. The plugin reads its bundled images from `CasinoSystem/Images` instead of downloading them.

Custom bot and currency images can use a data-relative path such as `CasinoSystem/Images/MyCurrency.png`. Custom HTTP URLs remain remote. Missing local files are logged without an automatic HTTP retry. Steam player avatars use the game's normal Steam image handling.

The source URLs and SHA256 hashes of the 11 CasinoSystem PNGs are recorded in `CasinoSystem/image-manifest.json`. Images retain their original rights. No plugin source, configuration, or player data belongs in this repository.
