# 🚀 ZERO 2 by pheonix14 - Release Notes (Version 1.3.0)

**Release Date:** June 28, 2026  
**Developer / Maintainer:** pheonix14 (GitHub)  
**Package Name:** `com.example.customdrawer`  
**App Label:** ZERO 2  
**Build Target:** Android 15 / SDK 35 (Min SDK 26)  

---

## 📌 Release Overview & Major Redesign (V1.3.0)
ZERO 2 Version 1.3.0 introduces a comprehensive UI redesign inspired by **Redmi HyperOS** and **Samsung One UI**, giving app icons full freedom without heavy circular backgrounds or artificial container boxes. This release also implements instant app loading performance and auto-adjusting system bar paddings.

---

## 🔥 Key Updates & Enhancements in V1.3.0

### 1. 📲 Redmi HyperOS & Samsung One UI Dock & Workspace
- **Clean Icon Freedom:** Removed heavy circular grey backgrounds behind app icons. Icons sit directly and vividly on your wallpaper.
- **Transparent Dock:** Eliminated the dark curved rectangle container behind hotseat dock apps for a clean, modern floating aesthetic.
- **System Insets Auto-Adjust:** Integrated `statusBarsPadding()` and `navigationBarsPadding()` across workspace and hotseat layouts so status bars and navigation gestures never cut off UI elements.

### 2. ⚡ Lightning-Fast App Loading Speed
- **In-Memory Caching:** Implemented thread-safe asynchronous app caching inside `AppLauncherEngine`. Subsequent drawer and grid renders load instantaneously without UI stuttering or lag.

### 3. 🔍 Custom Removable Search Bar
- **Draggable / Dismissable Search:** Replaced static weather headers with a clean, dismissable search widget featuring live filtering and instant response.

### 4. 🏷️ Clean Branding & UI Polish
- **Official App Name:** Updated app manifest label strictly to **ZERO 2**.
- **Header Cleanup:** Removed unnecessary floating action buttons from top right corners for a distraction-free home screen.

---

## 📦 Build Artifacts
- **Release APK:** `ZERO 2 V1.3.apk`
- **Version Code:** `4`
- **Version Name:** `1.3.0`
