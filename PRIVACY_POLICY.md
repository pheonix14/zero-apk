# Privacy Policy — Zero Launcher

**Last Updated**: June 26, 2026  
**Developer**: pheonix14 (github.com/pheonix14)  
**App Name**: Zero Launcher  
**Version**: 9.1  

---

## 1. Overview

Zero Launcher ("the App") is a free, open-source Android home screen launcher created entirely **for fun and personal use**. This privacy policy explains our data practices — specifically that we collect **none**.

---

## 2. What Data We Collect

**We collect absolutely nothing.**

Zero Launcher does **NOT**:

- ❌ Collect personal information (name, email, phone number, etc.)
- ❌ Track your location
- ❌ Access your contacts, call logs, or messages
- ❌ Record audio or video
- ❌ Upload any data to any server
- ❌ Use analytics, crash reporting, or telemetry
- ❌ Use advertising SDKs or track behavior
- ❌ Share data with third parties
- ❌ Store any data outside your device

---

## 3. Permissions Used & Why

Zero Launcher requests certain Android permissions. Here's exactly why each is needed:

| Permission | Why It's Needed |
|---|---|
| `QUERY_ALL_PACKAGES` | To display the list of installed apps on your home screen |
| `READ_CALENDAR` / `WRITE_CALENDAR` | For the calendar widget on the home screen |
| `INTERNET` | To optionally fetch Bing Daily Wallpaper (done locally, no data sent) |
| `ACCESS_NETWORK_STATE` / `ACCESS_WIFI_STATE` | To show Wi-Fi status in the quick toggles panel |
| `BLUETOOTH` | To show Bluetooth status in the quick toggles panel |
| `SET_WALLPAPER` | To set wallpaper via the System Wallpaper mode |
| `READ_EXTERNAL_STORAGE` / `READ_MEDIA_IMAGES` / `READ_MEDIA_VIDEO` / `READ_MEDIA_AUDIO` | To let you pick photos/videos for wallpaper and skins from your gallery |
| `POST_NOTIFICATIONS` | To show the foreground service notification (required by Android for overlay services) |
| `EXPAND_STATUS_BAR` | To expand the notification shade via gesture |
| `PACKAGE_USAGE_STATS` | To display recently used apps in the task switcher overlay |
| `VIBRATE` | For haptic feedback on button taps |
| `RECEIVE_BOOT_COMPLETED` | Reserved for potential future auto-start functionality |
| `SYSTEM_ALERT_WINDOW` | To draw overlays (volume panel, task switcher, gesture nav) on top of other apps |
| `FOREGROUND_SERVICE` | Required by Android to run the overlay engine in the background |
| `BIND_ACCESSIBILITY_SERVICE` | To enable custom back/recent gestures via the accessibility service |
| `MODIFY_AUDIO_SETTINGS` | To read current volume levels for the custom volume panel display |

All permissions are used **exclusively on-device** for launcher functionality. No data from any of these permissions is transmitted off your device.

---

## 4. Bing Daily Wallpaper

If you enable the **Bing Daily Wallpaper** feature, the app makes an outbound HTTP request to:

```
https://www.bing.com/HPImageArchive.aspx
```

This is a **one-way data fetch** — the app downloads a publicly available image URL from Microsoft Bing. Zero Launcher sends no user data, identifiers, or tracking information to Bing. This is equivalent to opening the Bing homepage in your browser.

---

## 5. Local Storage

Zero Launcher stores the following **only on your device**:

- Your settings and preferences (wallpaper mode, accent color, icon shape, etc.) — stored in Android SharedPreferences
- Wallpaper images you pick from your gallery — copied to app internal storage (`/data/data/com.example.projectzero/files/wallpapers/`) for persistent access
- Bing Daily Wallpaper image (cached locally)

All data is **private to the app** and accessible only on your device. It is deleted if you uninstall the app.

---

## 6. No Third-Party Services

Zero Launcher uses **no third-party SDKs** for analytics, advertising, crash reporting, or any purpose. The app does not integrate with:

- Google Analytics / Firebase Analytics
- Facebook SDK
- Crashlytics / Sentry / Bugsnag
- Any advertising network
- Any telemetry or tracking service

---

## 7. Children's Privacy

Zero Launcher does not knowingly collect information from children under 13. Since we collect no information from anyone, there is no risk to children's privacy.

---

## 8. Security

Since no data is transmitted to any server, there is no remote server to compromise. Your data stays on your device, protected by Android's standard security model.

---

## 9. Changes to This Policy

If this policy ever changes (e.g., if a new feature is added that requires data collection), the updated policy will be published in the GitHub repository and the update notes.

---

## 10. Contact

If you have any questions about this privacy policy, please open an issue at:

**https://github.com/pheonix14/project-zero/issues**

---

## 11. Summary

> 🛡️ **Zero Launcher collects zero data. Your phone, your files, your privacy — all stay with you.**

This app is built for fun. There is no business model, no monetization, and no incentive to collect anything. Enjoy the launcher!

---

*pheonix14 · github.com/pheonix14*
