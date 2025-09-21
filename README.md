# 🍎 Lenovo IdeaPad 130-15IKB Hackintosh - macOS Monterey 12.7.6

<div align="center">

![macOS Monterey](https://img.shields.io/badge/macOS-Monterey%2012.7.6-blueviolet?style=for-the-badge&logo=apple)
![OpenCore](https://img.shields.io/badge/OpenCore-1.0.5-blue?style=for-the-badge)
![Model](https://img.shields.io/badge/Model-IdeaPad%20130--15IKB-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Stable-success?style=for-the-badge)

**Complete EFI configuration for running macOS Monterey on Lenovo IdeaPad 130-15IKB (Type 81H7)**

*Hackintoshing: Because paying Apple premium prices is apparently optional* 😏

</div>

> ⚠️ **Use this repo only as a reference!** Please follow the official [Dortania OpenCore guide](https://dortania.github.io/OpenCore-Install-Guide/) for a proper Hackintosh setup. This repo shares only the EFI and hardware info for this particular model.

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

## ❌ Known Issues

- ❌ **Ethernet is slow** - Included [HoRNDIS](https://github.com/theQuert/HoRNDIS) for enabling USB tethering with android devices
- ❌ **Integrated WiFi and Bluetooth will not work**
- ❌ **Touchpad is wonky** - If you bring your finger close to the edge of the touchpad, cursor keeps moving until you swipe on the middle

## 📝 Notes

- 📝 **HDMI** - Not tested
- 📝 **SD Card Reader** - Not tested
- 📝 **This EFI has been tested up to Ventura 13.7.8 as it still supports Kaby Lake, but since Ventura is more optimized for Apple Silicon, Monterey is the most reliable choice.**

## ⚠️ Important Disclaimer

**Legal Notice:** 🚨 I am **NOT** responsible for thermonuclear war, Steve Jobs haunting your dreams, or Tim Cook sending hitmen to your home! 👻🍎 This is for **entertainment and educational reference only**. No warranty, no AppleCare, no Genius Bar for you! Use at your own risk, and **never blame me** for summoning ghostly software bugs or fruit-branded nightmares! 😱

**Hardware Warranty:** Hackintoshing may void your warranty faster than you can say "Genius Bar appointment." Proceed at your own risk, and maybe don't mention this to your local Apple Store employee. 🤫

**Support:** This is a community effort - Please do not expect official support from Apple, Lenovo, or your local tech support relative who "knows computers." 🤷‍♂️

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
