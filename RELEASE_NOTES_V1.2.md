# 🚀 ZERO 2 - Release Notes (Version 1.2.0)

**Release Date:** June 28, 2026  
**Developer / Maintainer:** pheonix14 (GitHub)  
**Package Name:** `com.example.customdrawer`  
**Build Target:** Android 15 / SDK 35 (Min SDK 26)  

---

## 📌 Release Overview & Summary
ZERO 2 Version 1.2.0 is a milestone update bringing major performance optimizations, structural stability enhancements, and refined launcher skin responsiveness. Built from the ground up to be lightweight and bloatware-free, V1.2 consolidates native Rust engine JNI bridges and delivers seamless app drawer animations.

---

## 🔥 Key Updates & Enhancements in V1.2.0

### 1. 🚀 Native Rust Engine Upgrade (`v1.2.0`)
- **Upgraded JNI Boundary:** Enhanced low-latency JNI bridge between Kotlin UI components and the high-performance Rust core (`native_core`).
- **Accelerated Search Filtering:** Multi-threaded query matching and optimized memory consumption when searching through installed applications.
- **Robust Fallback Engine:** Smart JVM fallback ensures zero crashes on devices with restricted native library permissions.

### 2. 🎨 Enhanced Launcher Skins & Dynamic UI
- **Zero Launcher Default:** Streamlined root workspace with instant access to hotseat apps and sliding bottom-sheet app drawer.
- **PS4 Dashboard & Futuristic Suite Sync:** Improved skin switching performance and smooth transition animations between drawer layouts.
- **Material 3 Dynamic Styling:** Fully tuned for Android 15 edge-to-edge rendering with dark color scheme optimization.

### 3. 🛠️ System Driver & Peripheral Daemon
- **Foreground Driver Service:** Stable background monitoring service for physical input devices, gamepads, and low-level peripheral event injection.
- **AppWidget Host Integration:** Reliable widget hosting lifecycle management with lifecycle-aware listening routines.

---

## 📦 Build Artifacts
- **Release APK Path:** `releases/ZERO 2 V1.2.apk` (and `app/build/outputs/apk/release/app-release.apk`)
- **Signing Status:** Signed with release/debug key for immediate installation on Android devices.
- **Version Code:** `3`
- **Version Name:** `1.2.0`

---
*Thank you for using ZERO 2! For issues, feedback, or contribution, visit the repository on GitHub.*
