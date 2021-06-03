
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


## Running perfectly but with some Err(0xE) messages at startup
00:000 00:000 AAPL: #[EB.H.IS|!] Err(0xE) <- RT.GV boot-signature 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:001 00:001 AAPL: #[EB.H.IS|!] Err(0xE) <- RT.GV boot-image-key 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:008 00:001 AAPL: #[EB.CFG.DEV|!] Err(0xE) <- RT.GV booter-strict-xmlparser 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:045 00:001 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.GV boot-signature 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:048 00:001 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.GV boot-image-key 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:051 00:001 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.GV boot-image 7C436110-AB2A-4BBB-A880-FE41995C9F82
00:053 00:001 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.SV- boot-signature 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:055 00:001 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.SV- boot-image-key 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:056 00:001 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.SV- boot-image 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:076 00:001 AAPL: #[EB.LD.OFS|OPEN!] Err(0xE) 

00:078 00:001 AAPL: #[EB.OPT.LXF|LF!] Err(0xE)

00:108 00:001 AAPL: #[EB.CS.CSKSD|!] Err(0xE) <- RT.GV boot-info-payload 8D63D4FE-BD3C-4AAD-881D-86FD974BC1DF

00:122 00:001 AAPL: #[EB.FS.AGSVH|!] Err(0xE) <- BS.LocHB 59D76AE4-37E3-55A7-B460-EF13D46E6020

00:135 00:001 AAPL: #[EB.WL.PWLFNV|!] Err(0xE) <- RT.GV wake-failure 7C436110-AB2A-4BBB-A880-FE41995C9F82

00:136 00:001 AAPL: #[EB.WL.DT|!] Err(0xE) <- EB.WL.PWLFNV

00:140 00:001 AAPL: #[EB.WL.DT|!] Err(0xE) <- EB.WL.PWLFRTC

00:146 00:002 AAPL: #[EB.LD.OFS|OPEN!] Err(0xE) 

01:759 00:001 AAPL: #[EB.B.WFDW|!WF] Err(0xE) 0


## Software:

-   [[Bootloader] OpenCore](https://github.com/acidanthera/OpenCorePkg)
-   [[Patch] AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
https://github.com/corpnewt/SSDTTime
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
