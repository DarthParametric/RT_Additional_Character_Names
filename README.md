# Additional Character Names
A mod for Owlcat's Rogue Trader cRPG. Adds additional random names for the RT and mercenaries in the character creator.

## Overview
This mod expands the available pool of randomly generated names in the character creator. By default, the game splits the available names into two pools: one for the player character, and one for mercenaries, resulting in only 30 available names for each sex in both pools. This mod joins both pools together and then adds a slew of additional names taken from a list [provided by Fantasy Flight](https://www.fantasyflightgames.com/ffg_content/rogue-trader-col-ed/Official-RT-names.pdf) as supplemental material for the original tabletop RT. After removing duplicates and common/unsuitable/uninteresting entries, this results in around 300 names for males and 125 for females.

## Installation
This is an Owlmod, made using the Unity template supplied by Owlcat. Currently the game has a bug that prevents Owlmods from working. To fix this, you ***must*** install the Unity Mod Manager-based mod [MicroPatches](https://github.com/microsoftenator2022/MicroPatches/releases) by microsoftenator2022. You can install it manually or via [ModFinder](https://www.nexusmods.com/warhammer40kroguetrader/mods/146).

To install this mod, first make sure you have run the game at least once. Download the archive and extract it into:

%LocalAppData%Low\Owlcat Games\Warhammer 40000 Rogue Trader\Modifications\
Each Owlmod needs to be in its own sub-folder in the Modifications folder.

Afterwards, you need to edit OwlcatModificationManagerSettings.json in the base Warhammer 40000 Rogue Trader folder in a text editor (Notepad++ recommended). It should look something like this:

```
{
"$id": "1",
"SourceDirectories": [],
"EnabledModifications": ["DPAdditionalCharacterNames"],
"ActiveModifications": ["DPAdditionalCharacterNames"],
"DisabledModifications": []
}
```

If you have other mods, list them in quotes separated by commas. For example:

```
"EnabledModifications": ["DPAdditionalCharacterNames", "ModName2", "ModName3"],
"ActiveModifications": ["DPAdditionalCharacterNames", "ModName2", "ModName3"],
```

You can move individual mods from the ActiveModifications section to the DisabledModifications section if you want to disable them without physically removing them.

Alternatively, use [ModFinder](https://www.nexusmods.com/warhammer40kroguetrader/mods/146) to install the mod.

It should be fine to install the mod in an existing game at any point, although obviously it's primarily intended for new games.

## Known Issues
This mod replaces the vanilla localisation strings for player/merc character names. As such, it is not compatible with any other mod that also replaces the same strings. GUIDs: `62681797-7835-4b5c-b8dd-63918881b28a` / `d109f177-8a63-40eb-8a51-dcd29d3eb94e` / `29e96169-b891-43ef-8b01-bf821656e4d7` / `566bb5f9-4e93-448a-b654-b9c2f2dc3efb`.

Currently the mod only replaces the names for the English localisation. Other languages will continue to use the vanilla set of names. If anyone wants to contribute localised versions in another language, let me know.

## Acknowledgements
Many thanks to the modders on the Owlcat Dicord, but particularly microsoftenator2022 and Kurufinve.
