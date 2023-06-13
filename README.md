# Hackintosh Configuration

This is my local OpenCore configuration for Ryzen 2600 & AM350

## Some things

- Used macOS: Ventura under MacPro7,1
- Patched for Six-core Processor
- Enabled 4G Decoding, SVM
- Disabled CSM, Secure Boot
- Disabled Secure Boot (solve exit code 2)

## Kexts

- [AMDRyzenCPUPowerManagement.kext](https://github.com/trulyspinach/SMCAMDProcessor)
- [AppleMCEReporterDisabler.kext](https://github.com/Pavo-IM/OC-Gen-X/issues/118)
- [Lilu.kext](https://github.com/acidanthera/Lilu)
- [NVMeFix.kext](https://github.com/acidanthera/NVMeFix)
- [RealtekRTL8111.kext](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [RestrictEvents.kext](https://github.com/acidanthera/RestrictEvents)
- [SMCAMDProcessor.kext](https://github.com/trulyspinach/SMCAMDProcessor)
- [VirtualSMC.kext](https://github.com/acidanthera/VirtualSMC/releases)
- [WhateverGreen.kext](https://github.com/acidanthera/WhateverGreen)
- [AppleALC.kext](https://github.com/acidanthera/AppleALC/releases)
**_Enabled only after installing OSX_**
- [USBToolBox.kext](https://github.com/USBToolBox/tool)
**_Replaced with USBMap.kext after mapping_**

## Utils

- [Gen SMBIOS](/Utils/Gen%20SMBIOS/)
  Used to generate System ProductName, SerialNumber, etc.

- [MAC Recovery](/Utils/MAC%20Recovery/)
  Used to generate Recovery Apple Image

- [Proper Tree](/Utils/Proper%20Tree/)
  Used to edit [config.plist](/EFI/OC/config.plist)
  
- [OC Validate](/Utils/OC%20Validate/)
  Used to recognize [config.plist](/EFI/OC/config.plist) errors

- [USBMap](/Utils/USBMap/)
  Used to create kext for USB Ports fix

## Using

You need to generate your own System Info with [Gen SMBIOS](/Utils/Gen%20SMBIOS/) for [config.plist](/EFI/OC/config.plist)
