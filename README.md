# Realtek UAD Edit
## Description
- This project provides custom drivers for Realtek chips (ALC210 - ALC1220).
- Supports Windows 10/11 x64 (Build 19041 or later).
## Features
- Dolby Atmos, DTS X Ultra, Nahimic support.
- APO1, APO2, and APO1 Legacy (SPDIF DDL/DTS) support.
## Installation
### Prerequisites
1. Uninstall existing Realtek drivers using [RAPR][DriverStoreExplorer].
2. Restart your PC.
### Generic/OEM Installation
1. Run `Install.cmd` or `Install_inf.cmd`.
2. Restart PC.
### OEM-Specific Installation
1. Remove `HDXRTKExt_APO1_RTK_PC.inf` from `Driver\UAD64\Realtek\ExtRtk_XXXX\`.
2. Copy:
   - From **ExtRtk_XXXX.7z**: `HDXRTKExt_XXXXXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX\`.
   - From **ThirdParty.7z**: `Dolby`, `DTS`, `A-Volute` folder to `Driver\UAD64\ThirdParty\`.
3. Configuration Examples:
   - **Generic:** `HDXRTKExt_XXXX_RTK_PC.inf`
   - **Dolby Atmos:** `HDXRTKExt_XXXX_DOLBY_PC.inf` + `Dolby` folder.
   - **DTS X Ultra:** `HDXRTKExt_XXXX_XPERI4_PC.inf` + `DTS` folder.
   - **Nahimic:** `HDXRTKExt_XXXX_AVO4_PC.inf` + `A-Volute` folder.
### Realtek APO1 Legacy (SPDIF DDL/DTS)
1. Remove `RealtekAPO_XXXX` from `Driver\UAD64\Realtek\`.
2. Copy `RealtekAPO_745` from **RealtekAPO_745_unlock.7z** to `Driver\UAD64\Realtek\`.
### Realtek APO2 Installation
1. Remove `HDXRTKExt_APO1_XXXXXXXXX.inf` and `RealtekAPO_XXXX` from `Driver\UAD64\Realtek\`.
2. Copy:
   - From **ExtRtk_XXXX.7z:** `HDXRTKExt_APO2_XXXXXXXXX.inf` to `Driver\UAD64\Realtek\ExtRtk_XXXX\`.
   - From **RealtekUAPO2_XXXX.7z:** `RealtekUAPO2_XXXX` to `Driver\UAD64\Realtek\`.
   - From **OVWrap2_XX.7z:** `OVWrap2_XX` to `Driver\UAD64\Realtek\`.
   - From **OVWrapN_XX.7z:** `OVWrapN_XX` to `Driver\UAD64\Realtek\`.

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
