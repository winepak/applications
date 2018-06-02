# Internet Explorer 8
Internet Explorer 8 is a web browser for the Microsoft Windows Operating System.

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  |       |
| 64bit | N/A      | N/A  |       |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.microsoft.InternetExplorer8.yml
    flatpak --user install winepak com.microsoft.InternetExplorer8

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.microsoft.InternetExplorer8.yml
    flatpak --user install winepak com.microsoft.InternetExplorer8

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.microsoft.InternetExplorer8.yml

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.microsoft.InternetExplorer8.yml

## Run

    flatpak run com.microsoft.InternetExplorer8

