# Win7-Chrome-DarkMode(DM4W7C)

---

# Win7-Chrome-DarkMode

**A zero-bloat solution to force-enable native Dark Mode on Google Chrome for Windows 7.**

## 💡 The Problem

On Windows 10/11, Chrome follows the system's dark theme automatically. However, **Windows 7** lacks the system-level APIs to toggle this, leaving users stuck with a blinding white interface. This repository provides a simple, clean bypass to unlock the native Chromium Dark engine.

---

## ✨ Features (核心特点)

* **Native Engine Activation**: Force-enables Chrome's hidden `WebContentsForceDark` and `ForceDarkMode` flags specifically for the Windows 7 environment.
* **No Extensions Required**: Unlike "Dark Reader," this uses Chrome's built-in rendering engine, saving CPU and RAM.
* **UI Persistence**: Fixes the issue where Chrome ignores theme settings on legacy operating systems.
* **Scrollbar & UI Patch**: Optimized CSS/Scripting to ensure the browser's internal pages (Settings, History) and scrollbars are also darkened.

---

## 🚀 Quick Start (快速开始)

### Method 1: The Shortcut Fix (Manual)

1. Right-click your Chrome shortcut and select **Properties**.
2. In the **Target** field, add the following to the very end:
```bash
--force-dark-mode --enable-features=WebContentsForceDark

```


3. Click **Apply** and restart Chrome.

### Method 2: One-Click Script (Source Included)

Run the `enable_dark_mode.bat` provided in this repository to automatically launch Chrome with the correct parameters.

---

## 🛠️ Source Contents (源码内容)

* **`scripts/enable_dark_mode.bat`**: The automation script to bypass Win7 theme limitations.
* **`src/`**: Contains the source logic for forcing dark UI elements and custom CSS patches for legacy builds.

---

## 📄 License

This project is licensed under the **MIT License**.

---
