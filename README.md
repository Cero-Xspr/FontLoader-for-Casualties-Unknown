# FontLoader-for-Casualties-Unknown

A BepInEx plugin that replaces the default game font with a custom TTF font for Casualties: Unknown.

Works alongside XUnity Auto Translator (Chinese localization mod) — the plugin has higher priority
so font blurring caused by Auto Translator's font replacement will be eliminated.

## Requirements

- **Casualties: Unknown** (Steam version)
- **BepInEx 5.x** (x64) installed in the game folder
- If install the **AutoTranslator** mod, need delete the "abc" in `OverrideFontTextMeshPro=abc` that in `/BepInEx/config/AutoTranslatorConfig.ini`

## Installation

1. Make sure BepInEx 5.x (x64) is installed in the game directory and works properly.
2. Copy `plugins/FontLoader.dll` into `BepInEx/plugins/` in your game folder.
3. Place **any `.ttf` font file** in the game root folder (next to `CasualtiesUnknown.exe`).
   The plugin will automatically find and load the first `.ttf` it finds.
4. Launch the game. The font will be applied automatically.

## Custom Font

Just drop any `.ttf` file into the game root folder. No specific filename needed.

## Compatibility

- Tested with Unity 2022.3.62f3 (Casualties: Unknown Demo)
- TMP (TextMeshPro) only — does not affect legacy GUI text

## License

MIT
