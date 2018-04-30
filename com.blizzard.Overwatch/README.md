# Overwatch
Competitive 6v6 team objective FPS

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  | No 32bit client available |
| 64bit | No       | N/A  | Need WoW64 support in Sdk/Platform |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.blizzard.Overwatch.json
    flatpak --user install winepak com.blizzard.Overwatch

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.blizzard.Overwatch.json
    flatpak --user install winepak com.blizzard.Overwatch

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.blizzard.Overwatch.json

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.blizzard.Overwatch.json

## Run

    flatpak run com.blizzard.Overwatch

