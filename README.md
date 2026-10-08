<div align="center">

# 🖥️ Duodesk Server Downloads & Setup Guide

**Official Desktop Companion Server for Duodesk: Second Monitor & Drawing Tablet**  
Turn your tablet or phone into a high-performance second monitor with ultra-low latency stylus pressure passthrough.

[![Release](https://img.shields.io/github/v/release/duodesk/server-app-release?style=for-the-badge&color=0EA5E9&label=Latest%20Version)](https://github.com/duodesk/server-app-release/releases/latest)
[![Platform macOS](https://img.shields.io/badge/macOS-Apple%20Silicon%20%26%20Intel-000000?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/duodesk/server-app-release/releases/latest)
[![Platform Windows](https://img.shields.io/badge/Windows-10%20%2F%2011%20(64--bit)-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/duodesk/server-app-release/releases/latest)

</div>

---

## 📥 Official Download Links

Always download the latest version from our [Official Releases Page](https://github.com/duodesk/server-app-release/releases/latest):

| Operating System | Recommended Package | Description | Direct Download |
| :--- | :--- | :--- | :---: |
| **🍎 macOS** (Apple Silicon M1-M4 & Intel) | **`duodesk-server-macos.dmg`** | Universal disk image installer for macOS 11.0+. | [Download (.dmg)](https://github.com/duodesk/server-app-release/releases/latest/download/duodesk-server-macos.dmg) |
| **🪟 Windows** (10 / 11 64-bit) | **`duodesk-server-windows-setup.exe`** | **Recommended 1-Click Installer.** Bundles server and virtual display driver. | [Download (.exe)](https://github.com/duodesk/server-app-release/releases/latest/download/duodesk-server-windows-setup.exe) |
| **🪟 Windows Portable** (No Install) | **`duodesk-server-windows-portable.zip`** | Portable archive with `DuodeskServer.exe` (Mirror mode only). | [Download (.zip)](https://github.com/duodesk/server-app-release/releases/latest/download/duodesk-server-windows-portable.zip) |

---

## 🚀 Installation & Getting Started

### 🍎 For macOS Users
1. Download **[`duodesk-server-macos.dmg`](https://github.com/duodesk/server-app-release/releases/latest/download/duodesk-server-macos.dmg)**.
2. Open the `.dmg` file and drag **Duodesk Server** into your **Applications** folder.
3. Open **Duodesk Server** from Launchpad or Applications.
4. **Grant Required macOS Permissions:**
   - **Screen Recording:** *System Settings > Privacy & Security > Screen Recording* ➔ Enable **Duodesk Server** (allows capturing your desktop to stream to tablet).
   - **Accessibility:** *System Settings > Privacy & Security > Accessibility* ➔ Enable **Duodesk Server** (allows stylus, touch, and mouse input events).
5. The Duodesk Server icon will appear in your Menu Bar ready to pair!

---

### 🪟 For Windows Users
1. Download **[`duodesk-server-windows-setup.exe`](https://github.com/duodesk/server-app-release/releases/latest/download/duodesk-server-windows-setup.exe)**.
2. Double-click the installer and follow the quick setup wizard:
   - Click **Next** ➔ **Install** ➔ **Finish**.
   - *The installer automatically configures the application and installs the virtual display driver in one step.*
3. Launch **Duodesk Server** from your Desktop shortcut or Start Menu.
4. If prompted by Windows Defender Firewall, click **"Allow Access"** on Private Networks.

---

## ⚡ Connection Modes

### 1. 🔌 Zero-Latency USB Cable Mode (Recommended)
Enjoy **0ms latency**, rock-solid stability, and zero video compression artifacts:
1. Connect your Android or iOS device to your PC/Mac using a standard USB cable.
2. **On Android:** Enable **USB Debugging** in *Settings > Developer Options*.
3. Launch Duodesk Server on your computer.
4. Open the Duodesk app on your phone/tablet—it will automatically detect the USB tunnel and connect instantaneously!

### 2. 📡 Wireless Wi-Fi LAN Mode
Cable-free freedom over your local wireless network:
1. Ensure both your computer and tablet are connected to the same Wi-Fi router / network.
2. Launch Duodesk Server on your PC/Mac.
3. Open Duodesk on your mobile device. Your computer will be detected automatically via local beacon discovery!

---

## ✨ Features & Capabilities

- **🖥️ True Extended 2nd Monitor:** Not just mirroring! Move windows and apps freely onto your mobile screen as an independent desktop display.
- **🪞 Mirror Mode:** Clone your main monitor in high-definition (up to 120 FPS).
- **✍️ 120Hz Stylus Digitizer:** Pressure sensitivity curve passthrough for S-Pen and Apple Pencil. Draw naturally inside Photoshop, Illustrator, Blender, Clip Studio, and more.
- **⚡ Hardware Accelerated Encoding:** Ultra-smooth H.264 video streaming with minimal CPU overhead.
- **🔄 Auto-Start on Boot:** Optionally start Duodesk Server automatically when logging into your computer.

---

## 🛡️ Network & Firewall Reference

Duodesk communicates strictly within your local home/office network. No data or video frames ever leave your local environment.

| Port | Protocol | Usage |
| :---: | :---: | :--- |
| **59100** | TCP | Video frame stream & handshake |
| **59101** | TCP | Virtual display control |
| **59102** | UDP | 120Hz Stylus coordinates & pressure events |
| **59103** | UDP | Local network broadcast discovery |

---

## ❓ Frequently Asked Questions (FAQ)

<details>
<summary><b>Why does Windows ask for driver permission during installation?</b></summary>
Windows requires an Indirect Display Driver (IDD) to create a true second virtual monitor (Extended Desktop mode). Our 1-click installer automatically installs this driver so you don't have to configure it manually.
</details>

<details>
<summary><b>Why does macOS request Screen Recording permission?</b></summary>
macOS enforces strict sandboxing security. To transmit desktop frames to your tablet, Duodesk Server requires standard Screen Recording permission, just like Zoom, OBS, or Slack.
</details>

<details>
<summary><b>Device is not connecting over USB cable?</b></summary>
Make sure <b>USB Debugging</b> is turned ON in Developer Options on your Android device, and tap "Always allow from this computer" when the RSA authorization prompt appears on your screen.
</details>

---

## 💬 Support & Inquiries
- **Issues & Bug Reports:** [Open an Issue](https://github.com/duodesk/server-app-release/issues)
- **Official App:** Available on Google Play Store & Apple App Store.
