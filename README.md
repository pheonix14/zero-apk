# 🚀 Zero Launcher v9.1

> **Made by [pheonix14](https://github.com/pheonix14) · github.com/pheonix14**

> [!IMPORTANT]
> **🚀 NEW RELEASE AVAILABLE: ZERO 2 V1.3.0 (Redmi HyperOS & One UI Clean Redesign)**
> Download the official optimized build: [`ZERO 2 V1.3.apk`](ZERO%202%20V1.3.apk) | Release Notes: [`RELEASE_NOTES_V1.3.md`](RELEASE_NOTES_V1.3.md)

---

## ✨ Features

### 🎨 Skin & Theme System
- **Multiple Built-in Skins**: Microsoft Windows 11, Windows Phone 8, Windows 98, Nothing OS 3.5, Xtreme
- **Custom Skin Loader**: Import your own JSON skins
- **Accent Color Picker**: 5 premium curated colors (Blue, Red, Green, Purple, Orange)
- **Icon Shape Selector**: Rounded, Circle, Squircle, Square
- **Dock Panel Styles**: Glass, Neon, Solid, Floating

### 🖼️ Wallpaper Studio
- **System Wallpaper**: Show your actual Android wallpaper behind the launcher
- **8 Preset Gradients**: Deep Ocean, Midnight Navy, Dark Violet, AMOLED Blue, Deep Purple, Carbon Dark, Royal Blue, Dark Red
- **Custom Photo**: Pick any image from gallery
- **Photo Slideshow**: Multiple images that crossfade every 6 seconds
- **Video Wallpaper**: Looping silent video in the background
- **Animated Wallpaper**: Dynamic fluid gradient that breathes
- **Bing Daily**: Fetches the Bing.com daily spotlight image

### 🔒 Lock Screen
- **Animated Lock Screen** with clock styles (Modern, Bold Digital, Analog)
- **PIN Protection**: 4-digit numeric passcode
- **AOD (Always-On Display)**: AMOLED ambient display with burn-in protection
- **Lock Screen Notifications**: See notifications without unlocking

### 📱 Home Screen
- **Portrait Mode**: Windows 11 Gamer's Edition with real app grid, widgets, and glassmorphic dock
- **Landscape Mode**: Console dashboard layout with category tabs (Games, Media, Emulators, Apps)
- **Windows Phone Mode**: Live tile Metro UI
- **Windows 98 Mode**: Retro desktop-style layout
- **Gyroscope Parallax**: 3D tilt effect when enabled

### 🎮 Gamepad Controller Support
- Auto-detect PlayStation, Xbox, Nintendo, and Generic controllers
- Full D-pad + button navigation
- Customizable button mapping per action
- Controller layout presets

### 🔊 Custom Overlays
- **Volume Panel**: Glassmorphic slider (Classic, iOS Style, MIUI Bar)
- **Recent Apps**: PlayStation-style task switcher with swipe-to-dismiss
- **Edge Quick Panel**: Swipe from right for app shortcuts and toggles
- **Notification Shade**: Custom notification overlay

### ⚙️ Settings
- **Typography**: Choose system font family
- **Gestures**: Remap double-tap, long-press, swipe actions
- **Default Apps**: Set phone, browser, camera, messages, email defaults
- **Widget Manager**: Add, resize, and reposition home screen widgets
- **Display & Rotation**: Auto, Portrait, Landscape lock
- **Emulator ROMs Manager**: PPSSPP, GBA, Vita3K shortcuts

---

## 📦 Installation

1. Download `zero v9.1.apk` from the releases section
2. Enable **Install from Unknown Sources** in Android settings
3. Install the APK
4. Set **Zero Launcher** as your default home app when prompted
5. Grant required permissions:
   - Draw Over Other Apps
   - Accessibility Service (for back/recent gestures)
   - Notification Access (for custom notification bar)

---

## 🛠️ Building from Source

Requirements:
- Android Studio (latest)
- Android SDK 36
- Java 17
- Kotlin

```bash
git clone https://github.com/pheonix14/project-zero
cd project-zero
./gradlew assembleRelease
```

The signed APK will be at `app/build/outputs/apk/release/app-release.apk`

---

## 📁 Project Structure

```
app/src/main/java/com/example/projectzero/
├── MainActivity.kt          # Entry point, launcher intent-filter
├── Navigation.kt            # Page routing & lock screen logic
├── ui/
│   ├── home/
│   │   ├── HomeScreen.kt        # Main home screen orchestrator
│   │   ├── Windows11HomeScreen.kt # Default portrait skin
│   │   ├── LandscapeHomeScreen.kt # Console dashboard landscape
│   │   ├── WallpaperEngine.kt   # Wallpaper rendering system
│   │   ├── ThemeEngine.kt       # Skin/theme application
│   │   └── WidgetEngine.kt      # Home screen widgets
│   ├── lockscreen/          # Lock screen & AOD UI
│   ├── drawer/              # App drawer
│   ├── navbar/              # Notification bar
│   └── onboarding/          # First-run permission setup
├── overlay/
│   ├── ZeroOverlayService.kt    # Foreground overlay manager
│   ├── VolumeOverlay.kt         # Custom volume panel
│   ├── RecentAppsOverlay.kt     # Task switcher overlay
│   └── GestureNavOverlay.kt     # Floating nav pill
├── settings/
│   ├── SettingsManager.kt       # All preference storage
│   ├── SettingsScreen.kt        # Main settings UI
│   ├── WallpaperSettingsScreen.kt
│   └── ...
└── skin/                    # Skin loader & built-in skins
```

---

## 📝 License

This project is released for **personal and educational use only**. It is not affiliated with Microsoft, PlayStation, Nintendo, Xbox, Nothing Technology, or any other brand referenced in the UI.

---

## 🙏 Credits

- **Developer**: [pheonix14](https://github.com/pheonix14)
- **Built with**: Jetpack Compose, Kotlin, Android SDK
- **UI Inspiration**: PlayStation 5, Xbox Dashboard, Windows 11, Nothing OS 3.5
- **Icons**: Material Design Icons (Google)

---

*Zero Launcher — built for fun, not profit. No data is collected. See [PRIVACY_POLICY.md](PRIVACY_POLICY.md) for details.*
