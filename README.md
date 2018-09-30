# HappyFotoFlatpak

Flatpak manifest for the HappyFoto-Designer App.

https://www.happyfoto.de/

## Installation

### Platform and Sdk
    flatpak remote-add --if-not-exists winepak https://dl.winepak.org/repo/winepak.flatpakrepo
	flatpak install winepak org.winepak.Platform/i386/3.0
	flatpak install winepak org.winepak.Sdk/i386/3.0

### Happy Foto
    flatpak-builder --arch=i386 --force-clean builds --repo=winepak de.happyfoto.happyfoto.yml
    flatpak --user install winepak de.happyfoto.happyfoto