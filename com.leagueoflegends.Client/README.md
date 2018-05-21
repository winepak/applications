# League of Legends
A Multiplayer Online Battle Arena Game

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | Yes      | Yes  | None  |
| 64bit | Yes      | Yes  | None  |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.leagueoflegends.Client.json
    flatpak --user install winepak com.leagueoflegends.Client
    
#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.leagueoflegends.Client.json
    flatpak --user install winepak com.leagueoflegends.Client

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.leagueoflegends.Client.json
    
#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.leagueoflegends.Client.json

## Run

    flatpak run com.leagueoflegends.Client

