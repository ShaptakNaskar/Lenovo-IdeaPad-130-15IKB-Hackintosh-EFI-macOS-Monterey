# 🍎 Lenovo IdeaPad 130-15IKB Hackintosh - macOS Monterey 12.7.6

<div align="center">

![macOS Monterey](https://img.shields.io/badge/macOS-Monterey%2012.7.6-blueviolet?style=for-the-badge&logo=apple)
![OpenCore](https://img.shields.io/badge/OpenCore-0.9.7-blue?style=for-the-badge)
![Model](https://img.shields.io/badge/Model-IdeaPad%20130--15IKB-red?style=for-the-badge&logo=lenovo)
![Status](https://img.shields.io/badge/Status-Stable-success?style=for-the-badge)

**Complete EFI configuration for running macOS Monterey on Lenovo IdeaPad 130-15IKB (Type 81H7)**

*Hackintoshing: Because paying Apple premium prices is apparently optional* 😏

</div>

## 📋 Hardware Specifications

| Component | Specification |
|-----------|---------------|
| **Model** | Lenovo IdeaPad 130-15IKB (Type 81H7) |
| **CPU** | Intel Core i5-7200U (Kaby Lake) |
| **GPU** | Intel HD Graphics 620 |
| **RAM** | 8GB DDR4 2400MHz (Upgradeable to 12GB) |
| **Storage** | 256GB M.2 SATA SSD + 1TB HDD |
| **Display** | 15.6" FHD (1920x1080) TN Panel |
| **Audio** | Conexant CX20751/2 |
| **Ethernet** | Realtek RTL8111 |
| **WiFi/BT** | Intel AC 3165 (Replaced with BCM94352Z DW1560) |
| **USB Ports** | 2x USB 3.0, 1x USB 2.0, 1x USB-C |
| **Other** | SD Card Reader, HDMI, VGA, 3.5mm Audio Jack |

## ✅ Working Components

- ✅ **macOS Monterey 12.7.6** - Fully functional
- ✅ **Intel HD Graphics 620** - Hardware acceleration, Metal support
- ✅ **Audio** - Internal speakers, headphone jack, microphone
- ✅ **Ethernet** - Realtek RTL8111 working perfectly
- ✅ **WiFi & Bluetooth** - BCM94352Z DW1560 (native support)
- ✅ **USB Ports** - All ports (USB 2.0, 3.0, USB-C)
- ✅ **Trackpad** - Full gesture support with I2C
- ✅ **Keyboard** - All keys including function keys
- ✅ **Display** - Native resolution, brightness control
- ✅ **Sleep/Wake** - Working properly
- ✅ **Power Management** - CPU frequency scaling
- ✅ **Battery** - Proper battery percentage and status
- ✅ **HDMI** - External display support
- ✅ **SD Card Reader** - Full functionality
- ✅ **Webcam** - Working with all apps

## ❌ Known Issues

- ❌ **VGA Port** - Not supported (hardware limitation)
- ❌ **Intel WiFi AC 3165** - Replaced with compatible card
- ⚠️ **Bluetooth Audio** - Occasional codec issues (minor)
- ⚠️ **Hibernation** - Disabled for stability

## 🛠 Pre-Installation Requirements

### Hardware Modifications
- **WiFi Card Upgrade**: Replace Intel AC 3165 with BCM94352Z DW1560
  - **Why?** Intel WiFi has limited macOS support
  - **Alternative**: Use USB WiFi dongle or Intel WiFi kexts (experimental)

### BIOS Settings
| Setting | Value |
|---------|-------|
| **Secure Boot** | Disabled |
| **Fast Boot** | Disabled |
| **Intel VT-d** | Disabled |
| **CSM Support** | Disabled |
| **UEFI Boot** | Enabled |
| **SATA Mode** | AHCI |

## 📦 EFI Configuration Details

### OpenCore Version
- **Version**: 0.9.7 (Latest stable)
- **Target**: macOS Monterey 12.7.6

### Key Kexts Used
- `Lilu.kext` - Patching engine
- `WhateverGreen.kext` - Graphics patches
- `AppleALC.kext` - Audio driver (layout-id: 3)
- `RealtekRTL8111.kext` - Ethernet driver
- `AirportBrcmFixup.kext` - BCM WiFi support
- `BrcmPatchRAM3.kext` - Bluetooth patches
- `VoodooPS2Controller.kext` - Keyboard/trackpad
- `VoodooI2C.kext` + `VoodooI2CHID.kext` - I2C trackpad
- `USBPorts.kext` - Custom USB port mapping
- `CPUFriend.kext` - CPU power management

### ACPI Patches
- `DSDT-HPET.aml` - HPET device fix
- `DSDT-EC.aml` - Embedded controller
- `DSDT-PLUG.aml` - CPU plugin type
- `DSDT-PNLF.aml` - Backlight control
- `DSDT-XOSI.aml` - OS compatibility

## 🚀 Installation Guide

### Step 1: Create macOS Installer
1. Download macOS Monterey 12.7.6 from App Store or Apple
2. Create bootable USB using `createinstallmedia` command
3. Copy EFI folder to USB EFI partition

### Step 2: BIOS Configuration
1. Enter BIOS setup (F2 during boot)
2. Apply settings from requirements table above
3. Save and exit

### Step 3: First Boot
1. Boot from USB installer
2. Use Disk Utility to format target drive as APFS
3. Install macOS following on-screen instructions
4. Copy EFI to system drive after installation

### Step 4: Post-Installation
1. Install Xcode Command Line Tools
2. Run essential kext installation commands
3. Configure iServices (optional)
4. Apply cosmetic tweaks

## ⚠️ Important Disclaimer

> **Legal Notice**: This project is for educational purposes only. macOS is proprietary software owned by Apple Inc. This EFI configuration does not contain any copyrighted Apple software. Users are responsible for obtaining legitimate copies of macOS and ensuring compliance with Apple's Software License Agreement.
> 
> **Hardware Warranty**: Hackintoshing may void your warranty faster than you can say "Genius Bar appointment." Proceed at your own risk, and maybe don't mention this to your local Apple Store employee. 🤫
> 
> **Support**: This is a community effort - no official support from Apple, Lenovo, or your local tech support relative who "knows computers."

## 📚 Useful Resources

### Essential Guides
- 📖 [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) - The holy grail
- 🔧 [OpenCore Post-Install](https://dortania.github.io/OpenCore-Post-Install/) - Polish your setup
- 🛠 [ProperTree](https://github.com/corpnewt/ProperTree) - config.plist editor
- 💻 [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) - Serial number generator

### Troubleshooting Resources
- 🆘 [r/Hackintosh Subreddit](https://www.reddit.com/r/hackintosh/)
- 💬 [Hackintosh Discord](https://discord.gg/hackintosh)
- 📝 [OpenCore Debugging](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/debug.html)
- 🔍 [Hackintool](https://github.com/headkaze/Hackintool) - System information utility

### Kaby Lake Specific
- 🏗 [Kaby Lake Guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.phtml/kaby-lake)
- ⚡ [CPU Power Management](https://dortania.github.io/OpenCore-Post-Install/universal/pm.html)
- 🎮 [Intel HD 620 Acceleration](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.phtml/kaby-lake#deviceproperties)

## 🤝 Contributing

Found improvements or fixes? Contributions are welcome!

1. Fork this repository
2. Create a feature branch
3. Test thoroughly on your hardware
4. Submit a pull request with detailed description

## 📜 Changelog

### v1.0.0 (Current)
- ✨ Initial release for macOS Monterey 12.7.6
- 🔧 Full hardware compatibility
- 📱 Complete USB port mapping
- 🎵 Working audio with all outputs
- 🌐 BCM94352Z WiFi/BT support
- 💤 Stable sleep/wake functionality

## 💝 Acknowledgments

- **OpenCore Team** - For the amazing bootloader
- **Dortania Team** - For comprehensive guides
- **Acidanthera** - For essential kexts
- **r/Hackintosh Community** - For endless support and coffee-fueled debugging sessions ☕

---

<div align="center">

**⭐ If this helped you, consider starring the repository!**

*Made with ❤️ and way too much caffeine*

![Visitors](https://visitor-badge.laobi.icu/badge?page_id=ShaptakNaskar.Lenovo-IdeaPad-130-15IKB-Hackintosh-EFI-macOS-Monterey)

</div>
