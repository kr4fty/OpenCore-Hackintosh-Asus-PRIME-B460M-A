# OpenCore Hackintosh for Asus PRIME B460M-A

[![macOS](https://img.shields.io/badge/macOS-11.6.1-orange)](https://web.archive.org/web/20211018064504/https://www.apple.com/macos/big-sur/)
[![macOS](https://img.shields.io/badge/macOS-12.0.1-orange)](https://www.apple.com/es/macos/monterey/)
[![macOS](https://img.shields.io/badge/macOS-13.4-orange)](https://www.apple.com/es/macos/ventura/)
[![macOS](https://img.shields.io/badge/macOS-14.5-orange)](https://www.apple.com/es/macos/ventura/)
[![OpenCore](https://img.shields.io/badge/OpenCore-1.0.6-9cf)](https://github.com/acidanthera/OpenCorePkg)

<img align="right" src="https://i.ibb.co/rHy5mN0/sonoma.png" alt="Critter" width="250">


**macOS Version supported/tested:**
 * ***11.6.1 [20G224]*** ✅
 * ***12.0.1 [21A559]*** ✅
 * ***13.4   [22F66]***  ✅
 * ***14.5   [23F79]***  ✅

**OpenCore Version:** ***[1.0.6 Official](https://github.com/acidanthera/OpenCorePkg/releases/tag/1.0.6)***

 *This OpenCore hackintosh repo is made for Asus PRIME B460M-A i5-10400 UHD630.*

<br />
<br />
<br />
<img align="center" src="https://i.ibb.co/GQ9DG5Y/Captura-de-pantalla-2024-06-10-a-la-s-9-59-20-p-m.png" alt="Critter" width="720">

## Configuration

| Specifications | Detail | Big Sur | Monterey | Ventura |Sonoma|
| :------------: | :------: | :--------: | :--------: | :--------: |:--------: |
| Motherboard | Asus PRIME B460M-A | ✅ | ✅ | ✅ |✅ |
| Processor | Intel® Core i5-10400 @ 2.90Ghz | ✅ | ✅ | ✅ |✅ |
| RAM | ADATA 3200MHz 8Gb | ✅ | ✅ | ✅ |✅ |
| HDD | SAMSUNG HD322HJ 320GB | ✅ | ✅ | ✅ |✅ |
| iGPU | Intel UHD Graphics 630 | ✅ | ✅ | ✅ |✅ |
| Sound Card | Realtek ALC 887 | ✅ | ✅ | ✅ |✅ |
| Ethernet Card | Realtek RTL8111H | ✅ | ✅ | ✅ |✅ |
| WiFi Card | Atheros AR9285 | ✅ | ✘ | ✘ |✘ |

## Working

- macOS 11.6.1 - 14.5
- CPU Boost
- iGPU
- Ethernet
- Audio
- USB
- WiFi (works up to Big Sur)

## Not Working

- WiFi Atheros: This kext generates a **Kernel panic** in Monterey and higher version
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
