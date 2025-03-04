# BO1-Microsoft-Changes
Some of the main differences between the Microsoft Store and Steam versions of Black Ops.

## Executables
- The game is now a 64 bit application, both executables are larger than Steam's.

### `BlackOps.exe`

Steam:

![image](https://github.com/user-attachments/assets/6e9484d8-3336-4336-8c6e-383830ef23e4)

Microsoft Store:

![image](https://github.com/user-attachments/assets/faafd129-58c1-4d74-bf11-ff512c70acc3)

### `BlackOpsMP.exe`

Steam:

![image](https://github.com/user-attachments/assets/b27328c8-1fa1-45cd-8e7f-846c34c193ce)

Microsoft Store:

![image](https://github.com/user-attachments/assets/a549f5c6-df79-45be-bf6a-e9c4fb826a17)

- No existing tools currently work.
- (Unconfirmed) This may affect box error.
- (Unconfirmed) Insta kill rounds likely do not exist.
- The check for restarting the map once the entities counter reaches `0x7ffffffd` (2,147,483,645) is unchanged. Many people know this as "reset".
- Much of the underlying code appears to be changed.

## Map Changes
- Some fastfiles are different in size, indicating things have been removed or added.
- None of the fastfiles can be extracted with any existing tools.

### `common_zombie_patch.ff` as an example:

Steam:

![image](https://github.com/user-attachments/assets/a10c60f1-43d1-40cd-948e-66780f0ed92d)

Microsoft Store:

![image](https://github.com/user-attachments/assets/d766c702-920d-45a3-aeba-e0fa270e0341)

- Sprinting zombies appear to run slightly faster.
- The World at War zombies maps contain entirely new map images on the main menu.

![image](https://github.com/user-attachments/assets/686adf29-a6eb-45ec-8dbf-c7b42ae9e806)

### Kino Der Toten
- The trap switches now have a very noticable glow.

![shot0002](https://github.com/user-attachments/assets/8ba1938d-4da8-4e63-9c64-8d56b5696cc9)

- The spawn teleporter pad is extremely shiny.

![shot0001](https://github.com/user-attachments/assets/335d16f2-c7d6-4626-9e05-502d67319ff7)

### Ascension
- The skybox has been completely replaced, screenshot taken on Steam with the extracted skybox texture.

![image](https://github.com/user-attachments/assets/aa24bd84-99dd-48cd-9b2f-ba65fba41445)

- The main menu image is the one from console.

![image](https://github.com/user-attachments/assets/03a6f123-2a01-44bb-8bfe-4b3d13866297)

- The files for contain concept art that we have never seen before.

![image](https://github.com/user-attachments/assets/a9fc7330-0bc4-4d1b-92bb-f498b38c2fd2)

![image](https://github.com/user-attachments/assets/6c203f2c-5e45-4b66-8963-112376926c43)

## CustomTextures/Camos
- Custom camos work just fine, those do not get reset.
- The `main` folder contains 60 `.iwd` files now, whereas Steam has `42`. These files contain over 9,000 new textures/sounds, some are duplicates (this is the same on Steam but not to this degree).
  - Some of the last modified dates of the files within these iwd archives go back as far as 2024.

## Config
- You can not edit the config as easily anymore, it will reset things you put in it that arent normally there after a system restart.
- Setting the config to read only mode will give you an `XGameSaveFilesGetFolderWithUiResult` error.

## Multiplayer
- The leaderboards appear to still have the developer/testing team stats on them.
- On the map "Jungle", the swamp is now completely blocked off with a fence as well as a rock next to the ladder walkway.

## Miscellaneous
- Connecting to a lobby on Zombies does not work.
- FPS will noticably decrease when all 24 zombies are on the map and being looked at.
