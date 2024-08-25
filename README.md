# Realtek UAD Edit Generic/OEM
### Motivation >
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
---
- Remove Driver\UAD64\Realtek\ExtRtk_9718.1\ `HDXRTKExt_RTK_PC.inf`
- #### Only one Ext/Folder
- Open Driver\UAD64\Realtek\ `ExtRtk_9718.1.7z`
- Place in Driver\UAD64\Realtek\ExtRtk_9718.1\
  > Dolby | DTS | Nahimic > `HDXRTKExt_DOLBY_PC.inf` | `HDXRTKExt_XPERI4_PC.inf` | `HDXRTKExt_AVO_PC.inf`
- Open Driver\UAD64\Realtek\ThirdParty.7z
- Place in Driver\UAD64\Realtek\ThirdParty\
  > Dolby | DTS | Nahimiс
---
- Run _CertTest/CertTest.bat(Admin)
- Installation via Driver/Setup.exe or Install.bat
- Restart PC
