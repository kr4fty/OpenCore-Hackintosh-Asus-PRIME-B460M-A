# OpenCore Hackintosh for Asus PRIME B460M-A

[![macOS](https://img.shields.io/badge/macOS-11.6.1-orange)](https://web.archive.org/web/20211018064504/https://www.apple.com/macos/big-sur/)
[![macOS](https://img.shields.io/badge/macOS-12.0.1-orange)](https://www.apple.com/es/macos/monterey/)
[![OpenCore](https://img.shields.io/badge/OpenCore-0.9.0-9cf)](https://github.com/acidanthera/OpenCorePkg)

<img align="right" src="https://i.ibb.co/T103KDc/del3rk1-177dea3e-01d6-4c32-bcfd-8927b7bc8364.png" alt="Critter" width="250">


**macOS Version supported/tested:**
 * ***11.6.1 [20G224]*** ✅
 * ***12.0.1 [21A559]*** ✅

**OpenCore Version:** ***[0.9.0 Official](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.0)***

 *This OpenCore hackintosh repo is made for Asus PRIME B460M-A i5-10400 UHD630.*

<br />
<br />
<br />
<img align="center" src="https://i.ibb.co/jMh8vDj/Captura-de-Pantalla-2021-12-07-a-la-s-14-25-05.png" alt="Critter" width="720">

## Configuration

| Specifications | Detail | Big Sur | Monterey |
| :------------: | :------: | :--------: | :--------: |
| Motherboard | Asus PRIME B460M-A | ✅ | ✅ |
| Processor | Intel® Core i5-10400 @ 2.90Ghz | ✅ | ✅ |
| RAM | ADATA 3200MHz 8Gb | ✅ | ✅ |
| HDD | SAMSUNG HD322HJ 320GB | ✅ | ✅ |
| iGPU | Intel UHD Graphics 630 | ✅ | ✅ |
| Sound Card | Realtek ALC 887 | ✅ | ✅ |
| Ethernet Card | Realtek RTL8111H | ✅ | ✅ |
| WiFi Card | Atheros AR9285 | ✅ | ✘ |

## Working

- macOS 11.6.1 - 12.0.1
- CPU Boost
- iGPU
- Ethernet
- Audio
- USB
- WiFi (works up to Big Sur)

## Not Working

- WiFi Atheros: This kext generates a **Kernel panic** in Monterey (12.0.1)
- ...

## BIOS Settings

 - Settings > Advanced > System Agent (SA) Configuration > VT-D: ***Disabled***
 - Settings > Advanced > USB Configuration > XHCI Hand-off: ***Enabled***
 - Settings > Advanced > PCI Subsystem Settings > Above 4G Decoding: ***Enabled***
 - Settings > Boot > CSM(Compatibility Support Module) > Launch CSM: ***Disabled***
 - Settings > Boot > Secure Boot > OS Type: ***Other OS***
 - Settings > Boot > Boot\Boot Configuration > Wait For 'F1' If Error: ***Disabled***

## Note

Please enter your codes (MLB, SystemSerialNumber, SystemUUID), into **config.plist** file

You can use this [guide](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo) as a reference

```
<dict>
    <key>AdviseWindows</key>
    <false/>
    <key>MaxBIOSVersion</key>
    <false/>
    <key>MLB</key>
    <string>ENTER HERE</string>
    <key>ProcessorType</key>
    <integer>0</integer>
    <key>ROM</key>
    <data>ESIzRFVm</data>
    <key>SpoofVendor</key>
    <true/>
    <key>SystemMemoryStatus</key>
    <string>Auto</string>
    <key>SystemProductName</key>
    <string>iMac20,1</string>
    <key>SystemSerialNumber</key>
    <string>ENTER HERE</string>
    <key>SystemUUID</key>
    <string>ENTER HERE</string>
</dict>
```

## References

- [dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [Fu-Yuxuan-hub](https://github.com/Fu-Yuxuan-hub/ASUS-TUF-GAMING-B460M-PLUS-HACKINTOSH)
- [tonyleelyy](https://github.com/tonyleelyy/OpenCore-Hackintosh-Asus-PRIME-B360M-A)
