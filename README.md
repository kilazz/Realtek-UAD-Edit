# Realtek UAD Edit Generic/OEM

## Compatibility
- **OS:** Windows 10/11 x64, version 19041 and above.
- **SoC:** ALC210-ALC1220 ~
- **Tested on:** A620M GAMING X AX (ALC897), etc.

## Removal
1. **Uninstall:** Remove the Realtek Audio Driver and related packages using [Rapr][DriverStoreExplorer].
2. **Restart:** Reboot your PC.

## Installation

### Generic/OEM Installation
1. **Run:** Execute `Install.cmd` or `Install_inf.cmd`.
2. **Restart:** Reboot your PC.

### OEM-Specific Installation
1. **Delete:** Remove `HDXRTKExt_RTK_PC.inf` from `Driver\UAD64\Realtek\ExtRtk_XXXX`.
2. **Extract and Copy:**
   - From **ExtRtk_XXXX.7z:** Copy `HDXRTKExt_XXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX`.
   - From **ThirdParty.7z:** Copy the `Dolby|DTS|A-Volute` folder to `Driver\UAD64\ThirdParty\`:
     - **Generic:** `HDXRTKExt_RTK_PC.inf`
     - **Dolby Atmos:** `HDXRTKExt_DOLBY_PC.inf` and the `Dolby` folder.
     - **DTS X Ultra:** `HDXRTKExt_XPERI4_PC.inf` and the `DTS` folder.
     - **Nahimic:** `HDXRTKExt_AVO4_PC.inf` and the `A-Volute` folder.

### Realtek APO1 or APO1 (Legacy) Unlocked SPDIF DDL/DTS
1. **Delete:** Remove `HDXRTKExt_APO2_RTK_PC.inf` from `Driver\UAD64\Realtek\ExtRtk_XXXX`.
2. **Extract and Copy:**
   - From **ExtRtk_XXXX.7z:** Copy `HDXRTKExt_APO1_XXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX`.
   - From **RealtekAPO_XXXX.7z** or **RealtekAPO_XXX_unlock.7z:** Copy `RealtekAPO_XXXX` or `RealtekAPO_XXX_unlock` to `Driver\UAD64\Realtek\`.

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
