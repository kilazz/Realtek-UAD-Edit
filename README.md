## Realtek UAD Edit Generic/OEM
#### Compatibility >
- Windows 10 x64 19041+
#### Removal >
- Uninstall Realtek Audio Driver and all packages, check via [Rapr][DriverStoreExplorer]
- Restart PC
#### Installation Generic/OEM >
- Unzip the archive .7z(Zstandard)
- Run _CertTest/`CertTest.bat`
- Installation using Driver/`Setup.exe` or `Install.bat`
- Restart PC
#### OEM >
- Delete    > Driver\UAD64\Realtek\ExtRtk_XXXX\ `HDXRTKExt_RTK_PC.inf`
- Open/Copy > `ExtRtk_XXXX.7z`|`ThirdParty.7z` > `HDXRTKExt_XXXXXXXXX.inf`|`OEM folder` >
- `Driver\UAD64\Realtek\ExtRtk_XXXX\`|`Driver\UAD64\ThirdParty\` >
  - `HDXRTKExt_RTK_PC.inf    |          > Generic`
  - `HDXRTKExt_DOLBY_PC.inf  | Dolby    > DolbyAtmos`
  - `HDXRTKExt_XPERI4_PC.inf | DTS      > DTSXUltra`
  - `HDXRTKExt_AVO4_PC.inf   | A-Volute > Nahimic`
#### ~ SPDIF 5.1 DDL/DTS (Legacy) >
- Delete    > Driver\UAD64\Realtek\ExtRtk_XXXX\ `HDXRTKExt_RTK_PC.inf`
- Open/Copy > `ExtRtk_XXXX.7z` > Driver\UAD64\Realtek\ExtRtk_XXXX\ `HDXRTKExt_APO1_XXXXXXXXX.inf`
- Delete    > Driver\UAD64\Realtek\ `RealtekUAPO2_XXXX`
- Open/Copy > `RealtekAPO_XXX_unlock.7z` > Driver\UAD64\Realtek\ `RealtekAPO_XXX_unlock`

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
