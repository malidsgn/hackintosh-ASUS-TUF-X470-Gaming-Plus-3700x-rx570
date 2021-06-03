
# hackintosh-ASUS-TUF-X470-Gaming-Plus-3700x-rx570
Sharing my hackintosh setup =D


## Tested Platform

-   ASUS TUF X470 Gaming Plus + AMD 3700X + RX570

## How to use

1. Download this repo and put EFI folder to your disk's EFI partition
2. Download OpenCore, go to OpenCore-x.y.z-RELEASE/Utilities, run ./macserial -a | grep iMacPro1,1 to generate Serial Number and MLB
3. Open EFI/OC/config.plist, copy && paste your generated Serial Number and MLB to PlatformInfo/Generic and PlatformInfo/SMBIOS
4. Change ROM to your network card's MAC address without the :, e.g: "06:d9:f6:1e:42:b6" => "06d9f61e42b6"
5. Boot your hackintosh!

## Software:

-   [[Bootloader] OpenCore](https://github.com/acidanthera/OpenCorePkg)
-   [[Patch] AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
-   [[Tool] SSDTTime](https://github.com/corpnewt/SSDTTime)
-   [[Driver] OpenRuntime](https://github.com/acidanthera/OpenCorePkg)
-   [[Driver] OpenCanopy](https://github.com/acidanthera/OpenCorePkg)
-   [[Driver] OpenHfsPlus](https://github.com/acidanthera/OpenCorePkg)
-   [[Kext] Lilu](https://github.com/acidanthera/Lilu)
-   [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
-   [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
-   [[Kext] AppleALC](https://github.com/acidanthera/AppleALC)
-   [[Kext] RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
-   [[Kext] AMDRyzenCPUPowerManagement](https://github.com/trulyspinach/SMCAMDProcessor)
-   [[Kext] SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)
-   [[Kext] NVMeFix](https://github.com/acidanthera/NVMeFix)
-   [[Kext] RestrictEvents](https://github.com/acidanthera/RestrictEvents)
-   [[Kext] AppleMCEReporterDisabler](https://github.com/AMD-OSX/AMD_Vanilla/blob/opencore/Extra/AppleMCEReporterDisabler.kext.zip)
## References
https://github.com/tylinux/hackintosh-ASUS-X570-Prime-Plus-3700x#how-to-use
