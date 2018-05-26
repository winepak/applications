# Notepad++
Source code editor

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | Yes      | Yes  | None  |
| 64bit | Yes      | Yes  | None |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak org.notepad_plus_plus.Notepad-plus-plus.yml
    flatpak --user install winepak org.notepad_plus_plus.Notepad-plus-plus
    
#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak org.notepad_plus_plus.Notepad-plus-plus.yml
    flatpak --user install winepak org.notepad_plus_plus.Notepad-plus-plus

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds org.notepad_plus_plus.Notepad-plus-plus.yml
    
#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds org.notepad_plus_plus.Notepad-plus-plus.yml

## Run

    flatpak run org.notepad_plus_plus.Notepad-plus-plus

