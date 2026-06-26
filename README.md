# Realtek UAD Edit

## Description
- Unofficial drivers for Realtek Audio chips (ALC210 - ALC1220).
- Windows 10/11 x64 (Build 19044 or later) support.

## Features
- Generic, DolbyAtmos, DTSXUltra, Nahimic support.
- Minimal & Default installation for Generic.
- Enhancements Tab support (`_MSAPO`).

## Installation

### Prerequisites
1. Uninstall existing Realtek drivers using [RAPR][DriverStoreExplorer].
2. Restart PC.

### Generic/OEM Installation
1. Run `RealtekUADInstaller.cmd` as Administrator (certificates will be imported automatically).
2. Select **Smart Clean** or **Force Clean** to remove old driver leftovers.
3. Select **Install Driver Set** and choose configuration.
4. Restart PC.

### Installation via Setup.exe
*Delete unwanted folders under `UAD64\ThirdParty` and excess `ExtRtk` INF files before running `setup.exe`.*
- **Generic**: `HDXRTKExt_APO2_RTK_EAA.inf`.
- **DolbyAtmos**: `HDXRTKExt_APO2_DOLBY_EAA.inf` + `Dolby` folder.
- **DTSXUltra**: `HDXRTKExt_APO2_XPERI4_EAA.inf` + `DTS` folder.
- **Nahimic**: `HDXRTKExt_APO2_AVO4_EAA.inf` + `A-Volute` folder.

## Troubleshooting
- **Windows Update**: Use **Toggle WU Driver Updates** and **Reset WU Cache & Ghost Devices** in the installer menu.
- **No Control Panel**: Ensure `RtkAudUService64.exe` is running at startup. Restart your PC if you change this setting.
- **DTS Issues**: If DTS does not work, restart the DTS service a few times.
- **Voice Call Volume Drop**: Win+R -> `mmsys.cpl` -> Communications tab -> Select "Do nothing".

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
