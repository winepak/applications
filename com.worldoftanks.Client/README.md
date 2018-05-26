# World of Tanks
A cult MMO game dedicated to armored machines

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | Yes      | No   | Installs, rest not tested |
| 64bit | No       | N/A  | Installs, rest not tested |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.worldoftanks.Client.yml
    flatpak --user install winepak com.worldoftanks.Client

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.worldoftanks.Client.yml
    flatpak --user install winepak com.worldoftanks.Client

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.worldoftanks.Client.yml

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.worldoftanks.Client.yml

## Run

    flatpak run com.worldoftanks.Client

