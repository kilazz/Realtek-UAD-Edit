## Realtek UAD Edit Generic/OEM
#### Compatibility >
- Windows 10/11 x64 19041+
- Only desktop motherboards were tested
#### Removal >
- Uninstall Realtek Audio Driver and all packages, check via [Rapr][DriverStoreExplorer]
- Restart PC
#### Installation Generic/OEM >
- Installation using `Install.cmd` or `Install_inf.cmd`
- Restart PC
#### OEM >
- Delete    > Driver\UAD64\Realtek\ExtRtk_XXXX\ `HDXRTKExt_RTK_PC.inf`
- Open/Copy > `ExtRtk_XXXX.7z`|`ThirdParty.7z` > `HDXRTKExt_XXXXXXXXX.inf`|`OEM folder` >
- `Driver\UAD64\Realtek\ExtRtk_XXXX\`|`Driver\UAD64\ThirdParty\` >
  - `HDXRTKExt_RTK_PC.inf    |          > Generic`
  - `HDXRTKExt_DOLBY_PC.inf  | Dolby    > DolbyAtmos`
  - `HDXRTKExt_XPERI4_PC.inf | DTS      > DTSXUltra`
  - `HDXRTKExt_AVO4_PC.inf   | A-Volute > Nahimic`
#### Realtek APO1/APO1 Legacy SPDIF DDL/DTS >
- Delete    > Driver\UAD64\Realtek\ExtRtk_XXXX\ `HDXRTKExt_APO2_RTK_PC.inf`
- Open/Copy > `ExtRtk_XXXX.7z` > Driver\UAD64\Realtek\ExtRtk_XXXX\ `HDXRTKExt_APO1_XXXXXXXXX.inf`
- Open/Copy > `RealtekAPO_XXXX.7z`/`RealtekAPO_XXX_unlock.7z` > Driver\UAD64\Realtek\ `RealtekAPO_XXXX`/`RealtekAPO_XXX_unlock`
#### Problems >
- You may need to restart DTS "DtsApo4Service" a few times after rebooting to get it working ~

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
