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
| **RAM** | 4GB single channel (upgraded to 8GB dual channel) |
| **Storage** | 1TB WD Blue HDD (upgraded to ADATA SU650 120GB SSD) |
| **Display** | 15.6" FHD (1920x1080) TN Panel |
| **Audio** | Realtek ALC236 |
| **Ethernet** | Realtek RTL810xE PCI Express Fast Ethernet controller (rev 07) |
| **WiFi/BT** | Wi-Fi: Realtek RTL8821CE 802.11ac PCIe Wireless, Bluetooth: Realtek 0bda:c024, RTL8821CE Combo Module |
| **USB Ports** | 2x USB 3.0 Ports (no EHCI since it's Kaby Lake) |
| **Other** | SD Card Reader, HDMI |

## ✅ Working Components

- ✅ **macOS Monterey 12.7.6** - Fully functional
- ✅ **Intel HD Graphics 620** - Hardware acceleration (only tested)
- ✅ **Audio** - Internal speakers, headphone jack, microphone
- ✅ **Ethernet** - Realtek RTL810xE working (see issues below)
- ✅ **USB Ports** - USB 3 only
- ✅ **Trackpad** - Full gesture support with I2C
- ✅ **Keyboard** - All keys including function keys
- ✅ **Display** - Native resolution, brightness control
- ✅ **Sleep/Wake** - Working properly
- ✅ **Power Management** - CPU frequency scaling
- ✅ **Battery** - Proper battery percentage and status
- ✅ **Webcam** - Working with all apps

## 📝 Notes

- 📝 **HDMI** - Not tested
- 📝 **SD Card Reader** - Not tested

## ❌ Known Issues

- ❌ **Ethernet is kinda slow** - Included Horndis for tethering with android
- ❌ **Integrated WiFi and Bluetooth will not work**
- ❌ **Touchpad is wonky** - If you bring your finger close to edge, cursor keeps moving until you swipe on the middle

## ⚠️ Important Disclaimer

**Legal Notice:** This project is for educational purposes only. macOS is proprietary software owned by Apple Inc. This EFI configuration does not contain any copyrighted Apple software. Users are responsible for obtaining legitimate copies of macOS and ensuring compliance with Apple's Software License Agreement.

**Hardware Warranty:** Hackintoshing may void your warranty faster than you can say "Genius Bar appointment." Proceed at your own risk, and maybe don't mention this to your local Apple Store employee. 🤫

**Support:** This is a community effort - no official support from Apple, Lenovo, or your local tech support relative who "knows computers."

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
- 🏗 [Kaby Lake Guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake)
- ⚡ [CPU Power Management](https://dortania.github.io/OpenCore-Post-Install/universal/pm.html)
- 🎮 [Intel HD 620 Acceleration](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake#deviceproperties)

## 🤝 Contributing

Found improvements or fixes? Contributions are welcome!

1. Fork this repository
2. Create a feature branch
3. Test thoroughly on your hardware
4. Submit a pull request with detailed description

## 💝 Acknowledgments

- **OpenCore Team** - For the amazing bootloader
- **Dortania Team** - For comprehensive guides
- **Acidanthera** - For essential kexts
- **r/Hackintosh Community** - For endless support and coffee-fueled debugging sessions ☕

⭐ If this helped you, consider starring the repository!

---

Made with ❤️ and way too much caffeine

![Visitors](https://visitor-badge.laobi.icu/badge?page_id=ShaptakNaskar.Lenovo-IdeaPad-130-15IKB-Hackintosh-EFI-macOS-Monterey)
