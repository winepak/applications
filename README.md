# Winepak Applications
A collection of flatpak manifest for building Microsoft Windows applications with Wine via flatpak.

## Instructions
Remember run all `flatpak` commands as a user, root and `sudo` are not needed.

### Sdk & Platform
First you need to build and install the winepak Sdk & Platform. You can do so at [winepak/winepak-sdk-images](https://github.com/winepak/winepak-sdk-images).

Some applications use the `stable` branch of `winepak` (which uses stable `wine`) while others use the `staging` branch of `winepak` (which uses `wine-staging`). Build the branches you'll need.

### Building an application
Now with the runtime installed we can build an application with `wine`. Flatpak will default the build to the systems arch, x86_64 = 64bit and i386 = 32bit. You can specify the arch by passing `--arch=ARCH`, remove this flag if you don't need it.

To build an application like `tld.domain.Application` we have two build options.

#### Repo
The repo version exports the build to a repo, in this case `winepak`. You then need to install the application via the local repo.

    flatpak-builder --arch=ARCH --force-clean --repo=winepak builds tld.domain.Application/tld.domain.Application.yml

Now to install simple run the application. Remember if you don't build the application with a GPG key then you will be forced to install the application with `--user`.

    flatpak install winepak tld.domain.Application

#### Direct
The direct method allows you to install a build directly from source without the need of a repo, this is done by running:

    flatpak-builder --user --arch=ARCH --force-clean --install builds tld.domain.Application/tld.domain.Application.yml

### Run the application
As easy as:

    flatpak run tld.domain.Application

