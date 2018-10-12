# HappyFotoFlatpak

Flatpak manifest for the HappyFoto-Designer App.

https://www.happyfoto.de/

## Installation

### Platform and Sdk
    flatpak remote-add --if-not-exists winepak https://dl.winepak.org/repo/winepak.flatpakrepo
	flatpak install winepak org.winepak.Platform/i386/3.0
	flatpak install winepak org.winepak.Sdk/i386/3.0

### Happy Foto
    flatpak-builder --repo=HappyFotoRepo --force-clean HappyFoto de.happyfoto.happyfoto.yml
	flatpak remote-add HappyFotoRepo HappyFotoRepo --no-gpg-verify
	flatpak install HappyFotoRepo de.happyfoto.happyfoto
