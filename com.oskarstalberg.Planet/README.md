# Polygonal Planet Project
A study in tilesets

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | Yes      | Yes  |       |
| 64bit | Yes      | Yes  |       |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean --repo=winepak builds com.oskarstalberg.Planet.yml
    flatpak --user install winepak com.pathofexile.Client
    
#### 64bit

    flatpak-builder --arch=x86_64 --force-clean --repo=winepak builds com.oskarstalberg.Planet.yml
    flatpak --user install winepak com.pathofexile.Client

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.oskarstalberg.Planet.yml
    
#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.oskarstalberg.Planet.yml

## Run

    flatpak run com.oskarstalberg.Planet

