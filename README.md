# Hackintosh Configuration

# STILL UNDER REVIEW!

This is my local OpenCore configuration for Ryzen 2600 & AM350

## Important Things

- Used Mac Version: MacPro7,1
- Patched for Six-core Processor
- Disabled Secure Boot (exit code 2)
- Enabled 4G Decoding, SVM
- Disabled CSM, Secure Boot

## Used Kexts

- [AppleALC.kext](https://github.com/acidanthera/AppleALC/releases)
**_Enable only after installing OSX_**
- [AMDRyzenCPUPowerManagement.kext](https://github.com/trulyspinach/SMCAMDProcessor)
- [AppleMCEReporterDisabler.kext](https://github.com/Pavo-IM/OC-Gen-X/issues/118)
- [Lilu.kext](https://github.com/acidanthera/Lilu)
- [NVMeFix.kext](https://github.com/acidanthera/NVMeFix)
- [RealtekRTL8111.kext](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [RestrictEvents.kext](https://github.com/acidanthera/RestrictEvents)
- [SMCAMDProcessor.kext](https://github.com/trulyspinach/SMCAMDProcessor)
- [USBToolBox.kext](https://github.com/USBToolBox/tool)
**_Replace to USBMap.kext after mapping_**
- [VirtualSMC.kext](https://github.com/acidanthera/VirtualSMC/releases)
- [WhateverGreen.kext](https://github.com/acidanthera/WhateverGreen)

## Used Utils

- [Gen SMBIOS](/Utils/Gen%20SMBIOS/)
  Used to generate System ProductName, SerialNumber, etc.

- [MAC Recovery](/Utils/MAC%20Recovery/)
  Used to generate Recovery Apple Image

  This is an example of how to download Ventura`s recovery: **_python3 ./macrecovery.py -b Mac-4B682C642B45593E -m 00000000000000000 download_**

  _This image will need to be written to the Apple HFS / HFS+ partition on USB Flash_

- [OC Validate](/Utils/OC%20Validate/)
  Used to recognize errors in the [config.plist](/EFI/OC/config.plist)

- [Proper Tree](/Utils/Proper%20Tree/)
  Used to edit [config.plist](/EFI/OC/config.plist)

- [USBMap](/Utils/USBMap/)
  Used to create kext for USB Ports fix

## Using

You need to generate your own System Info with [Gen SMBIOS](/Utils/Gen%20SMBIOS/) and write changes into [config.plist](/EFI/OC/config.plist)

Also, you need to correctly format USB Flash & write to it [EFI](/EFI/) and generated with [MAC Recovery](/Utils/MAC%20Recovery/) image
