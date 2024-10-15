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
- Delete > Driver\UAD64\Realtek\ExtRtk_XXXX.X\ `HDXRTKExt_RTK_PC.inf`
- Open   > `ExtRtk_XXXX.X.7z`|`ThirdParty.7z` >
- Copy   > `Only one HDXRTKExt_XXXXXXXXX.inf`|`Only one folder` > `Driver\UAD64\Realtek\ExtRtk_XXXX.X\`|`Driver\UAD64\ThirdParty\` >
  - `HDXRTKExt_DOLBY_PC.inf  | Dolby    > DolbyAtmos`
  - `HDXRTKExt_XPERI4_PC.inf | DTS      > DTSXUltra`
  - `HDXRTKExt_AVO4_PC.inf   | A-Volute > Nahimic`
- Run _CertTest/`CertTest.bat`
- Installation using Driver/`Setup.exe` or `Install.bat`
- Restart PC

[DriverStoreExplorer]: https://github.com/lostindark/DriverStoreExplorer
