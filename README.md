# ScreenMark - ITCG Screen Watermark Tool

> English | [中文](README_zh-CN.md)

**ScreenMark** is a professional screen watermark tool for Windows, designed to prevent information leaks through unauthorized photography and screenshots. It overlays customizable watermarks directly on the screen, providing a powerful visual deterrent against data theft.

**Version:** 3.3.7  
**Platform:** Windows 7+ (.NET 8.0)  
**License:** Free (Professional upgrade available)

---

## Features

### Four Watermark Types

| Type | Description | Availability |
|------|-------------|-------------|
| **Text Watermark** | Custom text with dynamic variables, fonts, colors | Free |
| **Image Watermark** | PNG/JPG/BMP image overlay | Pro |
| **3D Model Watermark** | GLB/GLTF/OBJ/STL/3DS 3D model display | Pro |
| **QR Code Watermark** | Dynamically generated QR codes | Pro |

### Dynamic Variables

Insert real-time dynamic variables into your watermark text that auto-refresh every second:

| Variable | Description |
|----------|-------------|
| `{username}` | Current Windows login username |
| `{ip}` | Local machine IPv4 address |
| `{hostname}` | Computer host name |
| `{mac}` | Network adapter MAC address |
| `{date}` | Current date (YYYY-MM-DD) |
| `{time}` | Current time (HH:mm:ss) |
| `{newline}` | Line break |

### Animation Effects

- **Horizontal Movement** — Watermark bounces left and right across the screen
- **Vertical Movement** — Watermark bounces up and down across the screen
- **Diagonal Movement** — Combine both directions simultaneously
- **Adjustable Speed** — 1-100 levels for precise control
- **Shadow Effects** — Drop shadow with configurable intensity

### Watermark Tiling

- Full-screen repeating watermark pattern to prevent photography and screenshots
- Configurable horizontal and vertical spacing for density control
- 45-degree text rotation for enhanced anti-tampering effect
- Uses WPF `VisualBrush` for high-performance rendering

### Desktop Background Overlay

- **Image Background** — Set a custom image as the full-screen background overlay
- **Color Background** — Solid color overlay with optional gradient effects
- **Gradient Modes** — Horizontal, vertical, or diagonal gradient directions
- Press **ESC** to cancel the background overlay

### 3D Model Watermark (Pro)

- Import 3D models in **GLB, GLTF, OBJ, STL, 3DS** formats
- Adjustable **scale** (0.1x-5x), **rotation speed** (0-180 deg/s), and **rotation axis** (X/Y/Z)
- Per-axis angle control (0-360 degrees)
- **Window size** configurable or **fullscreen fill** mode
- **Three lighting modes:**
  - **Simple** — Basic ambient + directional light
  - **Standard** — Three-point lighting (key, fill, rim)
  - **Cinematic** — Multi-light setup with warm/cool color contrast
- **Lighting controls:** specular reflection intensity, ambient light intensity, main light color/intensity
- **Edge light** and **dynamic rotating lighting** effects
- Built-in default 3D model included

### Multi-Monitor Support

- Detect all connected monitors
- Assign watermark to a specific screen
- Per-screen position and size configuration
- Refresh screen list at any time

### Preset Management

- Save complete watermark configurations as named presets (JSON format)
- **5 built-in presets** included:
  - Enterprise Leak Prevention
  - Personal Identification
  - Date & Time Stamp
  - Full Screen Tiling Anti-Photo
  - QR Code Traceability
- Load and switch presets instantly from settings or system tray
- Presets stored in `Presets/` directory for easy backup and sharing

### Security Password

- Set a security password to protect watermark settings
- Password required to open settings panel or exit the application
- Prevents unauthorized modification of watermark configuration

### Enterprise / Diskless Mode

Designed for enterprise environments with centralized IT management:

- **Per-Device Watermarks** — Assign unique watermarks to each machine by IP address
- **Common Watermark** — Shared watermark applied to all devices
- **Admin IP Restriction** — Only authorized IP addresses can modify settings
- **Batch Authorization** — Multi-device license management
- **Configuration File** — `EnterpriseConfiguration.ini` with IP-based rules

### Screen Focus Mode (Privacy Mask)

- Press `Ctrl + Shift + F` to toggle focus mode
- Active window stays bright with a **glowing border highlight**; the rest of the screen dims
- **Mouse-transparent** — click through the dimmed area to interact with windows underneath normally
- Highlight tracks the active window in **real time** as you switch or drag windows
- Configurable overlay opacity (20%–95%, default 70%) in System Settings
- Press `ESC` or `Ctrl + Shift + F` again to exit
- Multi-monitor support
- **Completely free** — no registration required

### USB Device Alert

- Real-time WMI-based detection for USB drives and external hard disks
- Unauthorized device insertion triggers a **system tray balloon notification** and log entry
- Captures full device details: drive letter, volume label, file system, capacity, hardware serial number, timestamp
- **Whitelist support** — company-issued drives added to the whitelist will not trigger alerts; match by serial number or drive letter
- One-click "Add Current Device" to whitelist, with manual editing and batch management
- Helps prevent internal data from being illegally copied via USB storage devices
- **Completely free** — no registration required

### Multi-Language Support

- **Chinese (zh-CN)** and **English (en-US)** full interface
- Auto-detects system language on first run
- Manual language switch available in System Settings at any time
- All settings panels, buttons, sliders, dropdowns, message boxes, and system tray menus fully translated

---

## Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Shift + O` | Open/Close settings panel |
| `Ctrl + Shift + F` | Toggle screen focus mode |
| `ESC` | Exit focus mode / Cancel background overlay |

---

## Pricing

| Edition | Features | Price |
|---------|----------|-------|
| **Free** | Text watermark, animation, tiling, presets, screen focus mode, USB alert, multi-language, all basic features | Free |
| **Professional** | Image watermark, 3D model watermark, QR code watermark, no ads | 18 CNY |

---

## Installation

### Requirements
- Windows 7 or later
- .NET 8.0 Runtime

### Download
Download the latest version from [https://sm.itcg.cn/](https://sm.itcg.cn/).

### Quick Start
1. Extract the ZIP archive
2. Run `ScreenMark.exe`
3. Right-click the system tray icon and select "Open Settings"
4. Configure your watermark text and settings
5. Click "Save & Close" to apply

---

## Feedback & Support

- Submit feedback via the built-in feedback form (Dashboard → Feedback)
- Submit feedback online at [https://hub.itcg.cn/user-dashboard/?tab=itcgFeedback](https://hub.itcg.cn/user-dashboard/?tab=itcgFeedback)

---

## License

Copyright © 2022-2024 ITCG. All rights reserved.

---

**ScreenMark** — Protect your screen, protect your data.
