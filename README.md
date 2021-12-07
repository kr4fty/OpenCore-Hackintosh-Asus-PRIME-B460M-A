# OpenCore Hackintosh for Asus PRIME B460M-A

[![macOS](https://img.shields.io/badge/macOS-11.6.1-orange)](https://web.archive.org/web/20211018064504/https://www.apple.com/macos/big-sur/)
[![macOS](https://img.shields.io/badge/macOS-12.0.1-orange)](https://www.apple.com/es/macos/monterey/)
[![OpenCore](https://img.shields.io/badge/OpenCore-0.7.5-9cf)](https://github.com/acidanthera/OpenCorePkg)

<img align="right" src="https://i.ibb.co/T103KDc/del3rk1-177dea3e-01d6-4c32-bcfd-8927b7bc8364.png" alt="Critter" width="250">


**macOS Version:**
 * ***11.6.1 [20G224]***
 * ***12.0.1 [21A559]***

**OpenCore Version:** ***[0.7.5 Offical](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.7.5)***

 *This OpenCore hackintosh repo is made for Asus PRIME B360M-A i5-10400 UHD630.*

 **Tested by: _@kr4fty_**
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

## Refrence

- [dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [Fu-Yuxuan-hub](https://github.com/Fu-Yuxuan-hub/ASUS-TUF-GAMING-B460M-PLUS-HACKINTOSH)
- [tonyleelyy](https://github.com/tonyleelyy/OpenCore-Hackintosh-Asus-PRIME-B360M-A)
