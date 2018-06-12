# StarCraft II
The Ultimate Real-time Strategy Game

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  |       |
| 64bit | Yes      | Yes  | Installs & runs with no issues; Only campaign was tested, not multiplayer |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.blizzard.StarCraft2.yml
    flatpak --user install winepak com.blizzard.StarCraft2

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.blizzard.StarCraft2.yml
    flatpak --user install winepak com.blizzard.StarCraft2

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.blizzard.StarCraft2.yml

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.blizzard.StarCraft2.yml

## Run

    flatpak run com.blizzard.StarCraft2

