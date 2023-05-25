# Hackintosh Configuration

### Roadmap

- Download [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg/releases) latest release

- Clone [ProperTree](https://github.com/corpnewt/ProperTree)

- Download latest MacOS recovery with macrecovery utility

**_python3 ./macrecovery.py -b Mac-4B682C642B45593E -m 00000000000000000 download_**

- Copy created com.apple.recovery.boot to USB flash

- Copy x64 OpenCore EFI to USB flash

- Clone [SSDTTime](https://github.com/corpnewt/SSDTTime)

- Create SSDT with SSDTTime and copy it to USB flash
