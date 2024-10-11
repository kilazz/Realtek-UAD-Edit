## Realtek UAD Edit Generic/OEM
#### Compatibility >
- Windows 10 x64 19041+
#### Removal >
- Uninstall Realtek Audio Driver and all packages, check via [Rapr][DriverStoreExplorer]
- Restart PC
#### Installation Generic >
- Unzip the archive .7z(Zstandard)
- Run _CertTest/`CertTest.bat`
- Installation using Driver/`Setup.exe` or `Install.bat`
- Restart PC
#### Installation OEM >
- Unzip the archive .7z(Zstandard)
- Delete > Driver\UAD64\Realtek\ExtRtk_XXXX.X/>
`HDXRTKExt_RTK_PC.inf`
- Open   > Driver\UAD64\Realtek\ `ExtRtk_XXXX.X.7z` > Place `Only one HDXRTKExt_XXXXXXXXXXX.inf` > Driver\UAD64\Realtek\ExtRtk_XXXX.X/>
`HDXRTKExt_DOLBY_PC.inf`
`HDXRTKExt_XPERI4_PC.inf`
`HDXRTKExt_AVO4_PC.inf`
`HDXRTKExt_AVO_PC.inf`
- Open   > Driver\UAD64\Realtek\ `ThirdParty.7z` > Place `Only one folder` > Driver\UAD64\Realtek\ThirdParty/>
`Dolby`
`DTS`
`A-Volute_Nh`
`A-Volute_SS3`
- Run _CertTest/`CertTest.bat`
- Installation using Driver/`Setup.exe` or `Install.bat`
- Restart PC

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
