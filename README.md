# MS-Store-BO1-Differences
Some of the main differences between the Microsoft Store and Steam versions of Black Ops.

- The game is now a 64 bit application, `BlackOps.exe` is over 1 MB larger than Steam's.
  - This means any existing tools will not work.
- All maps have be recompiled with different changes, the fastfiles are different in size, some are smaller and some are bigger.
  - Kino Der Toten has more noticable light glows on the trap switches.
  - The spawn teleporter pad is extremely shiny.
  - None of the fastfiles can be extracted with any existing tools.
  - This as well as the .exe changes could affect how many hits it takes to box error, still untested.
- The `main` folder contains 60 `.iwd` files now, whereas Steam has `42`. These files contain over 9,000 new textures/sounds, some are duplicates (this is the same on Steam but not to this degree).
  - Some of these files modified dates go back as far as 2024.
- You can not edit the config anymore, it will reset things you edit/put in it aside from what you can edit from the settings menu. Setting the config to read only will also give you an `XGameSaveFilesGetFolderWithUiResult` error.
- Sprinting zombies appear to run slightly faster.
- How things look as a whole appears to be different, some weapons have more details on them it seems.
- The underlying code appears to be vastly changed in some places.
- While reset has been untested, the check for restarting the map once the entities counter is about to reach `0x7ffffffd` (2,147,483,645) is unchanged.
- Connecting to a lobby on both Zombies and Multiplayer does not work.
- On the Multiplayer map "Jungle", the swamp is now completely blocked off with a fence as well as a rock next to the ladder path.
- The WAW zombies maps contain entirely new map images on the main menu.