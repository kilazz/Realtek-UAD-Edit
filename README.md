# Realtek UAD Edit Generic/OEM
### Motivation >
- For yourself ~
- Legacy support ~
- Forced upgrade ~
- Support OEM Ext Dolby/DTS/Nahimic ~
### Compatibility >
- Windows 10/11 18363/26090+
- Who knows
### Installation Generic >
- Uninstall Realtek Audio Driver and all packages, check via Rapr https://github.com/lostindark/DriverStoreExplorer
- Restart PC
- Unzip the .7z(Zstandard) archive
- Run _CertTest/CertTest.bat(Admin)
- Installation using Driver/Setup.exe or Install.bat
- Restart PC
### Installation OEM >
- Uninstall Realtek Audio Driver and all packages, check via Rapr https://github.com/lostindark/DriverStoreExplorer
- Restart PC
- Unzip the .7z(Zstandard) archive
- Delete Driver\UAD64\Realtek\ExtRtk_9718.1\ `HDXRTKExt_RTK_PC.inf`
- #### Place only one HDXRTKExt_ and one folder
  > Dolby | DTS | Nahimic >
  > `HDXRTKExt_DOLBY_PC.inf` | `HDXRTKExt_XPERI4_PC.inf` | `HDXRTKExt_AVO_PC.inf`
- Open Driver\UAD64\Realtek\ `ExtRtk_9718.1.7z` and place `HDXRTKExt_ .inf` in Driver\UAD64\Realtek\ExtRtk_9718.1\
- Open Driver\UAD64\Realtek\ `ThirdParty.7z` and place `OEM Folder` in Driver\UAD64\Realtek\ThirdParty\
- Run _CertTest/CertTest.bat(Admin)
- Installation using Driver/Setup.exe or Install.bat
- Restart PC
