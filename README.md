# Realtek UAD Edit

## Description
- This project provides unofficial drivers for Realtek Audio chips (ALC210 - ALC1220).
- Windows 10/11 x64 (Build 19041 or later) support.

## Features
- Generic, DolbyAtmos, DTSXUltra, Nahimic support.
- Enhancements Tab support. (except ExtRtkASPM)

## Installation

### Prerequisites
1. Uninstall existing Realtek Audio drivers using [RAPR][DriverStoreExplorer].
2. Restart PC.

### Generic/OEM Installation
1. Run `RealtekUADInstaller.cmd`.
2. Remove Drivers.
3. Install the required configuration.
4. Restart PC.

## Installation via Setup.exe

### Configuration example
1. **ExtRtk_XXXX** or **ExtRtkTest_XXXX**.
2. **Generic**: `HDXRTKExt_APO2_RTK_PC.inf`.
3. **Dolby Atmos**: `HDXRTKExt_APO2_DOLBY_PC.inf` + `Dolby` folder.
4. **DTS X Ultra**: `HDXRTKExt_APO2_XPERI4_PC.inf` + `DTS` folder.
5. **Nahimic**: `HDXRTKExt_APO2_AVO4_PC.inf` + `A-Volute` folder.
6. **Remove all unnecessary**.

## Troubleshooting
- Ensure the RtkAudUService64.exe service is enabled in your system's startup programs. Restart your PC if you change this setting.
- If DTS functionality is not working after installation, restart the DTS service.

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
