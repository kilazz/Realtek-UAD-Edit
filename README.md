## Realtek UAD Edit Generic/OEM

## Compatibility
- **OS:** Windows 10/11 x64, version 19041 and above
- **Tested on:** Desktop motherboards only ~

## Removal Steps
1. **Uninstall:** Realtek Audio Driver and packages using [Rapr][DriverStoreExplorer].
2. **Restart:** Reboot your PC.

## Installation Steps

### Generic/OEM Installation
1. **Run:** `Install.cmd` or `Install_inf.cmd`.
2. **Restart:** Reboot your PC.

### OEM-Specific Setup
1. **Delete:** `HDXRTKExt_RTK_PC.inf` from `Driver\UAD64\Realtek\ExtRtk_XXXX`.
2. **Extract and Copy:**
   - **ExtRtk_XXXX.7z:** Copy `HDXRTKExt_XXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX`.
   - **ThirdParty.7z:** Copy `OEM` folder to `Driver\UAD64\ThirdParty\`:
     - **Generic:** `HDXRTKExt_RTK_PC.inf`
     - **Dolby Atmos:** `HDXRTKExt_DOLBY_PC.inf`/`Dolby`
     - **DTS X Ultra:** `HDXRTKExt_XPERI4_PC.inf`/`DTS`
     - **Nahimic:** `HDXRTKExt_AVO4_PC.inf`/`A-Volute`

### Realtek APO1 or APO1 unlocked Legacy SPDIF DDL/DTS Setup
1. **Delete:** `HDXRTKExt_APO2_RTK_PC.inf` from `Driver\UAD64\Realtek\ExtRtk_XXXX`.
2. **Extract and Copy:**
   - **ExtRtk_XXXX.7z:** Copy `HDXRTKExt_APO1_XXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX`.
   - **RealtekAPO_XXXX.7z/RealtekAPO_XXX_unlock.7z:** Copy `RealtekAPO_XXXX` or `RealtekAPO_XXX_unlock` to `Driver\UAD64\Realtek\`.

## Troubleshooting
- **DTS Service:** Restart **DtsApo4Service** multiple times if needed. ~

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
