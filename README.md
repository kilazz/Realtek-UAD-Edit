# Realtek UAD Edit Generic/OEM
### Motivation >
- for myself ~
- Legacy Support/Force Updates ~
- Support OEM Ext Dolby/DTS/Nahimic etc ~
### Installation Generic >
- Remove Realtek Audio Driver and all packages, check via Rapr https://github.com/lostindark/DriverStoreExplorer
- Restart PC
- Unzip the archive .7z(Zstandard)
- Run _CertTest/CertTest.bat(Admin)
- Installation via Driver/Setup.exe or Install.bat
- Restart PC
### Installation OEM >
- Remove Realtek Audio Driver and all packages, check via Rapr https://github.com/lostindark/DriverStoreExplorer
- Restart PC
- Unzip the archive .7z(Zstandard)
- Remove Driver\UAD64\Realtek\ExtRtk_9718.1\ `HDXRTKExt_RTK_PC.inf`
- #### Place only one HDXRTKExt_ and Folder
  > Dolby | DTS | Nahimic >
  > `HDXRTKExt_DOLBY_PC.inf` | `HDXRTKExt_XPERI4_PC.inf` | `HDXRTKExt_AVO_PC.inf`
- Open Driver\UAD64\Realtek\ `ExtRtk_9718.1.7z` and place `HDXRTKExt_ .inf` in Driver\UAD64\Realtek\ExtRtk_9718.1\
- Open Driver\UAD64\Realtek\ `ThirdParty.7z` and place `OEM Folder` in Driver\UAD64\Realtek\ThirdParty\
- Run _CertTest/CertTest.bat(Admin)
- Installation via Driver/Setup.exe or Install.bat
- Restart PC
