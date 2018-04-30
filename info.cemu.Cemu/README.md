# Cemu
Nintendo Wii-U emulator

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  | No 32bit client available |
| 64bit | Yes      | Yes  |       |

## Build & Install
### Repo
#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak info.cemu.Cemu.json
    flatpak --user install winepak info.cemu.Cemu

### Direct
#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds info.cemu.Cemu.json

## Run

    flatpak run info.cemu.Cemu

