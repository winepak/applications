# Fortnite
Fortnite Battle Royale 100-player PVP

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  | No 32bit client available |
| 64bit | No       | N/A  | Need WoW64 support in Sdk/Platform |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.epicgames.Fortnite.json
    flatpak --user install winepak com.epicgames.Fortnite

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.epicgames.Fortnite.json
    flatpak --user install winepak com.epicgames.Fortnite

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.epicgames.Fortnite.json

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.epicgames.Fortnite.json

## Run

    flatpak run com.epicgames.Fortnite

