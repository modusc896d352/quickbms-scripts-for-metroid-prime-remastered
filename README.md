# quickbms-scripts-for-metroid-prime-remastered
self-explanatory

## rfrm.bms
What this script is is, in its current state, an asset exporter for RFRM files present in recent [Retro Studios](https://en.wikipedia.org/wiki/Retro_Studios) games, starting with **Donkey Kong Country: Tropical Freeze**.

### Compatibility
| Name of the Game | Usage Notes |
| --- | --- |
| **Donkey Kong Country: Tropical Freeze** | Multilated to shit. Don't expect any miracles. |
| **Metroid Prime Remastered** | Supports all known pak files from the outset. |

### Notes about RFRM format
The RFRM format can store just about any chunk, really. Here are the most prevalent ones so far.

Most files have an ADIR chunk where it acts as a listing of all available in-game assets from within what is called a "bigfile".

Said "bigfile" may have a bunch of textures, sounds, models and compiled scripts depending on the file. In any case, the ADIR chunk provides a lot of helpful pointers in case the game needs to access a particular asset to load.

What follows are optional META and STRG chunks, the former more prevalent than the other. The META chunk has all the metadata relating to a lot of in-game assets, and said metadata varies per asset. As for the STRG chunk, it simply provides an name for that asset.

**MaterialArchive.arc** is an unique case, however. This file is present across all games listed above and uses an entirely different set of chunks meant for loading materials from a part of an 3D model that requires such to be present in-game.

### Notes about using this script.
This script may require the latest quickBMS version available (get it [here](https://aluigi.altervista.org/quickbms.htm) first, you'll need it).

This script does not support compressed files from the outset. I do not know of a way to export them beyond doing so as-is and I do not have the adequate skill-set required to pull off such a feat.

# LICENSE (WIP)
rfrm.bms is free to use by just about anyone, really. For as long as you don't get me in trouble, that is.

# LEGAL (WIP)
This github repository has no relation to Nintendo, Retro Studios and all the companies who hold the rights to the above-mentioned games.

Said repository was made with academic research in mind and is not meant to harm anyone in any way.
