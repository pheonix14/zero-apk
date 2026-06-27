# ZERO 2 by pheonix14 — Release Notes V1.5.0
## "PS5 Full Console OS — Live Sync, Standalone Live Wallpaper & Deep Fidelity Update"

---

### 🎮 Overview
V1.5 is the most comprehensive ZERO 2 update yet — a full PS5 fidelity redesign addressing system bar cutouts, live app sync, wallpaper integration, standalone system live video wallpaper service, standalone widget hub, multi-font system, and performance across both portrait and landscape modes.

---

### 🔧 Bug Fixes & Enhancements

#### Display Cutout & System Bar Fixes
- **[CRITICAL FIX]** Replaced all `statusBarsPadding()` / `navigationBarsPadding()` with `WindowInsets.safeDrawing` — now correctly handles display notches, punch-holes, and nav bars in **both portrait and landscape** orientations
- `configChanges` added to AndroidManifest so rotation no longer triggers full Activity recreate
- PS5 Console Dashboard no longer forces landscape — now adaptive to both orientations
- `windowSoftInputMode="adjustNothing"` prevents layout jumps when keyboard appears

#### App Sync (Like Lawnchair)
- **[NEW]** Registered `LauncherApps.Callback` — launcher now **automatically detects** app installs, uninstalls, and updates in real-time without needing a manual refresh
- Apps list exposed as `StateFlow<List<AppInfo>>` — UI reacts to changes instantly
- Callback properly unregistered in `onDestroy()` to prevent memory leaks

#### Performance
- **[CRITICAL FIX]** Removed all blocking `toBitmap()` calls from `WorkspaceGrid`, `Hotseat`, and `Ps5ConsoleDashboard`
- All icons now loaded asynchronously via **Coil 2.7** with crossfade — zero main thread blocking
- Icon loading is cached by Coil's disk + memory cache automatically

---

### ✨ New Features

#### Standalone System Live Video Wallpaper Service (`WallpaperService`)
- **[NEW]** `ZeroLiveWallpaperService.kt` — Allows ZERO 2 to serve as an **Android System Live Wallpaper**! Even if you don't use ZERO 2 as your default launcher, you can activate ZERO 2 in system settings to run live video wallpapers across ANY launcher on your device.
- **[NEW]** Video Picker & Wallpaper configuration added to the interactive control center.

#### Standalone Widget Hub & Interactive Control Center
- **[NEW]** Dedicated Widget Dashboard mode supporting system app widgets (`AppWidgetHost`) with full D-Pad, Thumbstick, Controller buttons, Keyboard, and Mouse interaction.
- **[NEW]** Cleaned up top-right navbar — removed redundant search/settings icons for a sleek, authentic console aesthetic.

#### PS5 UI Full Fidelity
- **[NEW]** Top navigation bar matching PS5 reference: Games | Media pill tabs (left), Orbitron Clock + Avatar (right)
- **[NEW]** Activity cards show **large centered progress %** and **"In progress"** badge — exact PS5 UI
- **[NEW]** Card image blurred for non-focused items, sharp + scaled for focused card
- **[NEW]** Bottom PS5 system dock with 9 icons: Home, Notifications, Friends, Music, Volume, Mic, Controller, Storage, Power — with badge counts
- **[NEW]** **Friend Panel overlay** — matching PS5 reference image with avatar, online status, action icons, now-playing, and recently used apps

#### 5 PS5-Themed Fonts (Google Fonts)
- **Outfit** — Hero titles, card names, app headings
- **Inter** — Body text, app labels, subtitles
- **Orbitron** — Clock/HUD elements (gaming console aesthetic)
- **Rajdhani** — Metadata, progress text, secondary info
- **Oxanium** — Dock labels, tab items

#### Branding
- All screens consistently branded **"ZERO 2 by pheonix14"**
- Default launch mode is now PS5 Console Dashboard

---

### 📦 Technical Details
| Item | Value |
|------|-------|
| Version | 1.5.0 |
| Version Code | 6 |
| Min SDK | 26 (Android 8.0) |
| Target SDK | 35 (Android 15) |
| New Dependencies | Coil 2.7.0, Google Fonts, Palette |

---

### 📱 Installation
1. Download `ZERO 2 V1.5.apk`
2. Enable "Install from unknown sources"
3. Install and set as default Home app or enable as System Live Wallpaper

*Built with ❤️ by pheonix14 — Project ZERO 2*
