# Realtek UAD Edit
## Description
- This project provides custom drivers for Realtek Audio chips (ALC210 - ALC1220).
- Windows 10/11 x64 (Build 19041 or later) support.
## Features
- Generic, Dolby Atmos, DTS X Ultra, Nahimic support.
- APO1, APO2, and APO1 Legacy (SPDIF DDL/DTS) support.
- Enhancements Tab support.
## Installation
### Prerequisites
1. Uninstall existing Realtek Audio drivers using [RAPR][DriverStoreExplorer].
2. Restart PC.
### Generic/OEM Installation
1. Run `RealtekUADInstaller.ps1`.
2. Choose the required configuration.
3. Restart PC.
## Installation via Setup.exe
### OEM-Specific Configuration
1. **Generic**: Use `HDXRTKExt_APO1_RTK_PC.inf` or `HDXRTKExt_APO2_RTK_PC.inf`.
2. **Dolby Atmos**: Use `HDXRTKExt_APO1_DOLBY_PC.inf` or `HDXRTKExt_APO2_DOLBY_PC.inf` + `Dolby` folder.
3. **DTS X Ultra**: Use `HDXRTKExt_APO1_XPERI4_PC.inf` or `HDXRTKExt_APO2_XPERI4_PC.inf` + `DTS` folder.
4. **Nahimic**: Use `HDXRTKExt_APO1_AVO4_PC.inf` or `HDXRTKExt_APO2_AVO4_PC.inf` + `A-Volute` folder.
### Realtek APO1 Legacy (SPDIF DDL/DTS)
1. Replace `RealtekAPO_XXXX` with `RealtekAPO_745` in `Driver\UAD64\Realtek\`.

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
