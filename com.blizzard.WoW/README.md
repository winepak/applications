# World of Warcraft
Massively-multiplayer online role-playing game

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  | Dropping 32bit soon |
| 64bit | Yes      | N/A  | Battle.net installs; game not tested |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.blizzard.WoW.yml
    flatpak --user install winepak com.blizzard.WoW

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.blizzard.WoW.yml
    flatpak --user install winepak com.blizzard.WoW

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.blizzard.WoW.yml

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.blizzard.WoW.yml

## Run

    flatpak run com.blizzard.WoW

