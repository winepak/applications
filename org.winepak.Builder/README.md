# Winepak Builder
Winepak Builder tool

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | Yes      | Yes  | None  |
| 64bit | Yes      | Yes  | None  |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak org.winepak.Builders.json
    flatpak --user install winepak org.winepak.Builders
    
#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak org.winepak.Builders.json
    flatpak --user install winepak org.winepak.Builders

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds org.winepak.Builders.json
    
#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds org.winepak.Builders.json

## Run

    flatpak run org.winepak.Builders

