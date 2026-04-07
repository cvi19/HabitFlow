# 🌿 HabitFlow

A calm, wellness-focused Android habit tracker app. Build habits that actually stick, one day at a time.

## Features
- ✅ Track daily habits with a single tap
- 🔥 Streak tracking — see your consecutive days
- 🎨 Custom emoji icons for each habit
- 📴 Fully offline — no internet or account needed
- 🔒 Private by design — data stored only on your device

---

## Getting Started

### Prerequisites
- [Android Studio](https://developer.android.com/studio) (Hedgehog or newer)
- JDK 17+

### Clone & Open
```bash
git clone https://github.com/YOUR_USERNAME/HabitFlow.git
cd HabitFlow
```
Open in Android Studio → **File → Open** → select the `HabitFlow` folder.

### Build the APK

**From Android Studio:**
1. Wait for Gradle sync to complete
2. Go to **Build → Build Bundle(s) / APK(s) → Build APK(s)**
3. APK will be at: `app/build/outputs/apk/debug/app-debug.apk`

**From the terminal:**
```bash
chmod +x gradlew
./gradlew assembleDebug
```

---

## GitHub Actions — Automatic APK Builds

Every push to `main` or `master` automatically builds both debug and release APKs.

1. Push your code to GitHub
2. Go to **Actions** tab in your repo
3. Click the latest workflow run
4. Download the APK from the **Artifacts** section

---

## Project Structure

```
app/src/main/
├── java/com/habitflow/app/
│   ├── Habit.kt              # Data model
│   ├── HabitsStorage.kt      # SharedPreferences persistence
│   ├── HabitAdapter.kt       # RecyclerView adapter
│   ├── MainActivity.kt       # Home screen
│   └── AddHabitActivity.kt   # Add new habit screen
└── res/
    ├── layout/               # XML layouts
    ├── drawable/             # Shapes & icons
    ├── values/               # Colors, strings, themes
    └── mipmap-anydpi-v26/    # App launcher icon
```

## Requirements
- **Min SDK:** Android 8.0 (API 26)
- **Target SDK:** Android 14 (API 34)

---

Built with ❤️ using Kotlin + Material Components.
