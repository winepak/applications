# World of Tanks
A cult MMO game dedicated to armored machines

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  | None  |
| 64bit | No       | N/A  | Need WoW64 support in Sdk/Platform |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.worldoftanks.Client.json
    flatpak --user install winepak com.worldoftanks.Client

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.worldoftanks.Client.json
    flatpak --user install winepak com.worldoftanks.Client

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.worldoftanks.Client.json

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.worldoftanks.Client.json

## Run

    flatpak run com.worldoftanks.Client

