# 🍎 Lenovo IdeaPad 130-15IKB Hackintosh - macOS Monterey 12.7.6

<div align="center">

![macOS Monterey](https://img.shields.io/badge/macOS-Monterey%2012.7.6-blueviolet?style=for-the-badge&logo=apple)
![OpenCore](https://img.shields.io/badge/OpenCore-1.0.5-blue?style=for-the-badge)
![Model](https://img.shields.io/badge/Model-IdeaPad%20130--15IKB-red?style=for-the-badge)
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
| **RAM** | 4GiB single channel (upgraded to 8GiB dual channel) |
| **Storage** | 1TB WD Blue HDD (upgraded to ADATA SU650 120GB SSD) |
| **Display** | 15.6" FHD (1920x1080) TN Panel |
| **Audio** | Realtek ALC236 |
| **Ethernet** | Realtek RTL810xE PCI Express Fast Ethernet controller (rev 07) |
| **WiFi/BT** | Wi-Fi: Realtek RTL8821CE 802.11ac PCIe Wireless Combo Module |
| **USB Ports** | 2x USB 3.0 Ports |
| **Other** | SD Card Reader, HDMI |

## ✅ Working Components

- ✅ **Intel HD Graphics 620** - Hardware acceleration 
- ✅ **Audio** - Internal speakers, headphone jack, microphone
- ✅ **Ethernet** - Realtek RTL810xE working (see issues below)
- ✅ **USB Ports** - Both USB Ports working
- ✅ **Trackpad** - Basic functionality works
- ✅ **Keyboard** - All keys except Num Lock key (Numeric Keypad still works)
- ✅ **Display** - Native resolution, brightness control
- ✅ **Sleep/Wake** - Working properly
- ✅ **Battery** - Proper battery percentage
- ✅ **Webcam** - Working with all apps

## 📝 Notes

- 📝 **HDMI** - Not tested
- 📝 **SD Card Reader** - Not tested

## ❌ Known Issues

- ❌ **Ethernet is slow** - Included [HoRNDIS](https://github.com/theQuert/HoRNDIS) for enabling USB tethering with android devices
- ❌ **Integrated WiFi and Bluetooth will not work**
- ❌ **Touchpad is wonky** - If you bring your finger close to the edge of the touchpad, cursor keeps moving until you swipe on the middle

## ⚠️ Important Disclaimer

**Legal Notice:** This project is for educational purposes only. macOS is proprietary software owned by Apple Inc. This EFI configuration does not contain any copyrighted Apple software. Users are responsible for obtaining legitimate copies of macOS and ensuring compliance with Apple's Software License Agreement.

**Hardware Warranty:** Hackintoshing may void your warranty faster than you can say "Genius Bar appointment." Proceed at your own risk, and maybe don't mention this to your local Apple Store employee. 🤫

**Support:** This is a community effort - no official support from Apple, Lenovo, or your local tech support relative who "knows computers."

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
