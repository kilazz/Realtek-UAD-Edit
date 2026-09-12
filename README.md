# Realtek UAD | STRIX SOAR/RAID PRO/DLX Edit

## Description
- Unofficial drivers for Realtek Audio chips (ALC210 - ALC1220) and ASUS Strix SOAR/RAID PRO/DLX.
- Windows 10/11 x64 (Build 19044 or later) support.

## Features
- Default/Generic, Nahimic, DolbyAtmos, DTSXUltra, DTSVirtualX support.
- Minimal/Default installation for Generic (Realtek).
- Enhancements Tab support (`_MSAPO`).

## Installation

### For Realtek:
1. Uninstall existing Realtek drivers using [RAPR][DriverStoreExplorer].
2. Restart PC.
3. Run **`AudioInstaller.cmd`** as Administrator.
4. Select **`Realtek UAD Audio`**.
5. Select **Smart Clean** or **Force Clean** to remove old driver leftovers.
6. Select **Install Driver Set** and choose configuration.
7. Restart PC.

### For ASUS Strix:
1. Install `ASMedia_USB3x_1.16.61.1` (optional: High DPC Latency. Use Microsoft driver) ~
2. Install `Strix_Soar_Setup_1.1.23`.
3. Uninstall existing `nhAsusSC150/nhAsusSC200.inf` drivers using [RAPR][DriverStoreExplorer].
4. Run **`AudioInstaller.cmd`** as Administrator.
4. Select **`ASUS Strix Sound Card`**.
5. Select **Smart Clean** or **Force Clean** to remove old driver leftovers.
6. Select **Install Driver Set** and choose configuration.
7. Restart PC.

## Troubleshooting
- **No Control Panel**: Ensure `RtkAudUService64.exe` is running at startup. Restart your PC if you change this setting.
- **Audio App Issues**: If an app shows an error, restart its corresponding service (`DolbyDAXAPI`, `DtsApo4Service`, `DtsHubService`, `NahimicService`) in Task Manager or Services.
- **Windows Update**: Use **Toggle Windows Update Driver Downloads** and **Reset WU Cache & Clean Ghost Devices** in the installer menu.
- **Voice Call Volume Drop**: Win+R -> `mmsys.cpl` -> Communications tab -> Select "Do nothing".

## Store Applications
- After installing the driver, open the `.url` shortcuts inside the `Apps` folder to install the corresponding control panels from the Microsoft Store.

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
