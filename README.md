# GTA SA: It Never Ends: Mission Pack
Source codes of CLEO mission pack for GTA San Andreas released back in 2010 and patched in 2015. Three extra missions have been added as well, which are not included here, but can be found in a seperate repository: https://github.com/MakG10/gta-sa-it-never-ends-extras

## About the mod
The story is an extension of GTA San Andreas, it begins right where original storyline ended. A short in-sight: Carl's brother, Sweet, has been kidnapped by a mafia led by Bill Degorio and now CJ is forced to work for them.

Mission pack GTA SA: It Never Ends is consisted of:
- 11 missions, 8 of which with voiced dialogues
- 8 unique jumps
- 8 money bags to collect
- Cover System
- Autosave mechanism

## About the code
Mission pack was written in SCM language using Sanny Builder as an IDE and compiler. CLEO library was used to make a mod as an extension to the game without overwriting existing files.

`src/CLEO/ine.txt` file is a starter script. It executed after loading a game and contains all necessary logic not directly related to missions. It handles progress information, creating mission markers when not on mission, events in between missions, collectable bags, in-game mod menu (after typing "inemenu") and so on.

`src/CLEO/INE` folder contains all mission files which compile tu Custom Mission files (.cm). They are called from `ine.cs` explained above.

`src/CLEO/INE/mission_includes.txt` file contains some functions shared across missions source codes.

`src/CLEO/INE/global_header.txt` file contains variable mappings for `ine.cs`

`src/CLEO/CLEO_TEXT` folder contains translated strings used in the scripts.

## Tools
[Sanny Builder 3](https://sannybuilder.com/index.html) - IDE for SCM language
[mta2scm](http://www.gta-mods.pl/mta2scm) - self-made online tool for converting MTA map files into SCM code. Useful when creating large scenes with lots of actors, cars and objects.

## Authors and contributors
- MakG
- Silent
- LotNICK
- Przemysław 'primo' Lament
- CaptainFalcon
- Kuba
- krolikk
- Frixion
- Rosman
