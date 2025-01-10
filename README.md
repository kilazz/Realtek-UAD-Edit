## Realtek UAD Edit Generic/OEM

## Compatibility
- **Supported OS:** Windows 10/11 x64, version 19041 and above
- **Tested on:** Desktop motherboards only

## Removal Steps
1. **Uninstall:** Realtek Audio Driver and all related packages using [Rapr][DriverStoreExplorer].
2. **Restart PC:** Reboot your computer.

## Installation Steps

### Generic/OEM Installation
1. **Run:** `Install.cmd` or `Install_inf.cmd`.
2. **Restart PC:** Reboot your computer.

### OEM-Specific Setup
1. **Delete:** `HDXRTKExt_RTK_PC.inf` from `Driver\UAD64\Realtek\ExtRtk_XXXX`.
2. **Extract and Copy:**
   - **ExtRtk_XXXX.7z:** Copy `HDXRTKExt_XXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX`.
   - **ThirdParty.7z:** Copy `OEM` folder to `Driver\UAD64\ThirdParty\`:
     - **Generic:** `HDXRTKExt_RTK_PC.inf`
     - **Dolby Atmos:** `HDXRTKExt_DOLBY_PC.inf`
     - **DTS X Ultra:** `HDXRTKExt_XPERI4_PC.inf`
     - **Nahimic:** `HDXRTKExt_AVO4_PC.inf`

### Realtek APO1/APO1 Legacy SPDIF DDL/DTS Setup
1. **Delete** `HDXRTKExt_APO2_RTK_PC.inf` from `Driver\UAD64\Realtek\ExtRtk_XXXX`.
2. **Extract and Copy:**
   - **ExtRtk_XXXX.7z:** Copy `HDXRTKExt_APO1_XXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX`.
   - **RealtekAPO_XXXX.7z/RealtekAPO_XXX_unlock.7z:** Copy files to `Driver\UAD64\Realtek\RealtekAPO_XXXX` or `RealtekAPO_XXX_unlock`.

## Troubleshooting
- **DTS Service:** Restart **DtsApo4Service** multiple times if needed after rebooting. ~

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
