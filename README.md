# ATHLETIQ AI — Intelligent & Sovereign Fitness & Posture Coach

<div align="center">

![Platform](https://img.shields.io/badge/Platform-Android_8.0%2B-3DDC84?logo=android&logoColor=white)
![Price](https://img.shields.io/badge/Access-100%25_Free-2E7D32)
![Subscription](https://img.shields.io/badge/Subscription-None-brightgreen)
![Privacy](https://img.shields.io/badge/Data-100%25_Local_&_Sovereign-blue)
![Languages](https://img.shields.io/badge/Languages-EN_|_FR_|_ES_|_DE_|_IT_|_PT-orange)
[![Download APK](https://img.shields.io/badge/Download-APK_v1.0.0-C6F36A?logo=android&logoColor=black)](https://github.com/SammyYohan/AthletiqAI/releases/latest)

**The intelligent, privacy-first, 100% free bodybuilding & workout app with real-time AI camera posture coaching, deterministic program generation, and zero subscription paywalls.**

**English** • [Français](README.fr.md) • [Español](README.es.md) • [Deutsch](README.de.md) • [Italiano](README.it.md) • [Português](README.pt.md)

[Direct APK Download](#-download--installation-android) • [All Features](#-all-features-in-depth) • [A Word from Sammy Yohan](#-a-word-from-the-creator--sammy-yohan) • [Support the Project](#-support-the-project-ko-fi--paypal) • [Tech Stack](#-technical-architecture)

</div>

---

## 💬 A Word from the Creator — Sammy Yohan

> *"Hi everyone,*
> 
> *My name is Sammy Yohan. I have no venture capital, no investors, and zero marketing budget. I started with nothing in my pocket—just raw ideas, determination, and a passion for crafting software that genuinely helps people.*
> 
> *I built **ATHLETIQ AI** from scratch on my old personal computer. My core goal is simple: put cutting-edge technology (on-device computer vision, real-time biomechanical posture correction, metabolic calculations, and custom periodized training) into the hands of every lifter and fitness enthusiast, without any financial gatekeeping.*
> 
> *That is why **ATHLETIQ AI is and will always remain 100% free**. No paywalls, no subscriptions, no locked features, and no annoying ad pop-ups.*
> 
> *Right now, the app is **available exclusively on Android**. Why? Simply because I cannot afford a MacBook yet (which is required to build and compile with Apple's Xcode), nor can I afford Apple's annual developer fee ($99/year) or the initial Google Play developer console fee.*
> 
> *If ATHLETIQ AI helps you level up your training, correct your technique, or transform your physique, any support on Ko-fi or PayPal directly empowers me to keep building, publish officially to the Google Play Store, and eventually port the app to iOS once I can get my hands on a second-hand Mac.*
> 
> *Thank you from the bottom of my heart for your trust and support!"*
> 
> — **Sammy Yohan**

---

## 📥 Download & Installation (Android)

ATHLETIQ AI is distributed as a signed, ready-to-run APK release.

👉 **[Download ATHLETIQ AI v1.0.0 (APK)](https://github.com/SammyYohan/AthletiqAI/releases/latest)**

### How to Install in 3 Steps:
1. Download **`AthletiqAI-v1.0.0.apk`** from the [Releases](https://github.com/SammyYohan/AthletiqAI/releases/latest) page onto your Android device.
2. Open the downloaded file. If prompted by Android, enable *"Install from unknown sources"* for your browser or file manager.
3. Tap **Install** and start training immediately—no account creation or internet connection required!

> 📱 **Compatibility**: Android 8.0 (Oreo, API 26) and above (tested and optimized up to Android 15 & 16). Works 100% offline.

---

## ✨ All Features In-Depth

ATHLETIQ AI combines a native, high-performance UI (built with Kotlin and Jetpack Compose Material 3) with an advanced biomechanical engine:

### 1. 🎯 Comprehensive Biomechanical Onboarding
- **Zero-Friction Setup**: No cloud account or email required; your profile is created on-device in seconds.
- **Physical Parameters**: Age, height, and weight (full support for both Metric `kg/cm` and Imperial `lbs/in`).
- **Goal Selection**:
  - *Hypertrophy*: Target maximum muscle mass gains.
  - *Strength*: Prioritize progressive overload on compound lifts.
  - *Conditioning & Lean Definition*: High work capacity, fat loss, and definition.
  - *Technique & Posture*: Master movement mechanics and injury prevention.
  - *Rehabilitation / Gradual Return*: Safe return after a hiatus or injury.
- **Equipment & Location Calibration**:
  - Home Bodyweight / Calisthenics.
  - Minimal Equipment (Dumbbells, resistance bands, pull-up bar).
  - Full Commercial Gym (Barbells, power racks, adjustable benches, cables, and machines).
- **Custom Schedule & Volume**: Select between **1 to 7 training days per week** and tune workout duration from **25 to 90 minutes** (the engine automatically adjusts exercise selection and volume accordingly).
- **Lagging Muscle Prioritization**: Select specific muscle groups you want to bring up (Chest, Shoulders, Back, Biceps, Triceps, Abs, Quads, Glutes, Calves).

---

### 2. 🧠 Algorithmic Program Engine (`ProgramEngine`)
- **Deterministic & Instant**: Generates fully structured workout splits locally in milliseconds without server delays.
- **Adaptive Splits**:
  - *Full Body*: Balanced stimulation for 1 to 3 weekly sessions.
  - *Upper / Lower*: Ideal 4-day frequency for strength and recovery.
  - *Push / Pull / Legs (PPL)*: High-frequency hypertrophy split for 3 to 6 days.
  - *Arnold Split / Specialized Splits*: Advanced volume distribution.
- **Weak Point Specialization**: Lagging muscles are prioritized early in the session with prime neuromuscular activation.
- **Intelligent Rep Ranges & Tempos**:
  - 5–8 reps for heavy mechanical tension (Strength).
  - 8–12 reps for metabolic stress and hypertrophy.
  - 12–15+ reps for muscular endurance and bodyweight control.

---

### 3. 👁️ Real-Time AI Camera Posture Coach (MediaPipe Tasks Vision)
- **100% On-Device Computer Vision**: Powered by Google's MediaPipe Tasks Vision (`pose_landmarker_lite.task`), running directly on your phone's CPU/GPU.
- **3D Landmark Tracking**: Continuous tracking of 33 anatomical keypoints across knees, hips, shoulders, elbows, wrists, and ankles.
- **Finite State Rep Counter (`RepPhase`)**:
  - Automatic state transitions: `TOP` ➔ `DESCENDING` (controlled eccentric phase) ➔ `BOTTOM` (target depth) ➔ `ASCENDING` (concentric drive).
  - Full range of motion (ROM) verification: excludes cheated or half repetitions.
- **Real-Time Audio Feedback (`ToneGenerator`)**:
  - Pleasant chime on every successfully completed, clean repetition.
  - Distinct warning tone if movement breaks form or fails depth criteria.
- **Injury Prevention Module (Anti-Tear & Joint Safety)**:
  - *Knee Valgus Detection*: Warns when knees cave inwards on squats or lunges.
  - *Spine Alignment*: Detects excessive lumbar hyperextension or lower back rounding (*butt wink*).
  - *Elbow Flare Protection*: Enforces a safe ~45° pressing angle on push-ups to preserve the rotator cuff.
- **Front & Rear Camera Flexibility**: Switch instantly to front camera for real-time selfie-mirror mode or rear camera on a tripod/stand.
- **Manual Counter Fallback**: Audio clicker mode available when training without camera support or in low-light environments.

---

### 4. ⚡ Active Workout Tracker
- **Set-by-Set Guided Execution**: Live displays for target load, reps, and pacing.
- **Rapid Weight Increment Controls**: Quick `+ / - 2.5 kg` and `+ / - 5 kg` buttons (or lbs equivalent).
- **RPE Borg Scale Selector**: Log Rate of Perceived Exertion (1 to 10) to gauge proximity to failure (RIR).
- **Automated Rest Timer**: Starts immediately upon set completion, with sound notifications, rapid `+30s` button, and skip option.
- **Smart On-The-Fly Exercise Substitutions**: Gym bench taken? Swap any exercise in 1 tap for an anatomically equivalent regression or progression.
- **Crash & Interruption Resilience**: Every rep and set is automatically saved locally; resume seamlessly if interrupted by a call or app switch.
- **Comprehensive Post-Workout Summary**: Net session duration, cumulative tonnage lifted, sets completed, personal notes, and XP earned.

---

### 5. 📸 360° Video & Photo Body Scan
- **Multi-Angle Capture**: Guided front, side, and rear photos, or seamless 360° video scans.
- **Gallery Import**: Analyze existing fitness progress photos or videos directly from your phone.
- **9-Zone Anatomical Analysis**: Visual scoring across Shoulders, Chest, Back, Biceps, Triceps, Abs, Quads, Glutes, and Calves.
- **Symmetry & Weak Point Identification**: Numerical scores (0–100) and scan-to-scan delta progression tracking.
- **100% Sovereign Privacy**: Photos, videos, and biometric data **never leave your device**. No cloud uploads, no third-party AI inspection.

---

### 6. 🥗 Metabolic & Macro Nutrition Calculator
- **Physiological BMR**: Calculated using the clinically verified **Mifflin-St Jeor** formula.
- **Dynamic TDEE**: Activity factor dynamically calibrated to your actual weekly workout frequency and average session duration.
- **Automated Caloric Targets**:
  - *Lean Cut / Fat Loss*: Controlled deficit (-350 kcal/day) sparing lean muscle tissue.
  - *Hypertrophy / Clean Bulk*: Anabolic surplus (+250 kcal/day) minimizing fat gain.
  - *Strength*: Performance-focused surplus (+200 kcal/day).
  - *Recomposition / Maintenance*: Optimal energy balance.
- **Macro Distribution**:
  - *Proteins*: 1.7 to 2.1 g per kg of bodyweight.
  - *Fats*: ~0.95 g per kg for optimal hormonal and joint health.
  - *Carbohydrates*: Balanced to fuel heavy training sessions.
- **Personalized Hydration**: Daily water targets tailored to body mass and training volume.
- **Recovery Guidelines**: Science-based tips for pre/post-workout nutrition, sleep architecture, and central nervous system recovery.

---

### 7. 📈 Progression, History & Personal Records (PR)
- **Interactive Progress Charts**: Dynamic volume and frequency filters over 4, 8, and 12-week windows.
- **Personal Records Board (PR)**: Automatic estimated 1RM calculations and rep records for every lift.
- **30-Day Rolling Tonnage**: Visual metric to ensure consistent progressive overload.
- **Unlimited Workout Logs**: Revisit every past workout, complete with weight, reps, sets, and notes.
- **Bodyweight Tracking**: Monitor long-term weight evolution alongside workout data.

---

### 8. 🏆 Gamified Athlete Ranks & XP System
- **Dynamic Rank Evolution**:
  - 🥉 **Rank 1**: *Iron Novice*
  - 🥉 **Rank 2**: *Barbell Initiate*
  - 🥈 **Rank 3**: *Hypertrophy Practitioner*
  - 🥈 **Rank 4**: *V-Taper Sculptor*
  - 🥇 **Rank 5**: *Strength Master*
  - 🏆 **Rank 6**: *Athletic Titan*
- **Experience Points (XP)**: Earn XP for completed workouts, camera-verified reps, and regular body scans.

---

### 9. 📚 Comprehensive Exercise Library
- **Categorized by Muscle Group**: Chest, Back, Shoulders, Arms, Legs, Core.
- **Equipment Filters**: Bodyweight, Dumbbells, Barbells, Cables, Machines, Resistance Bands.
- **In-Depth Movement Guides**:
  - Step-by-step setup and execution cues.
  - Common biomechanical pitfalls and injury risks.
  - Accessible regressions (easier variants).
  - Challenging progressions (harder variants).
  - Muscle-matched substitutions.
- **One-Tap AI Coach Launch**: Jump straight into camera coaching for any supported movement.

---

### 10. 🌍 Multilingual by Design
- Fully translated and native in **6 major languages**:
  - 🇬🇧 English
  - 🇫🇷 French (Français)
  - 🇪🇸 Spanish (Español)
  - 🇩🇪 German (Deutsch)
  - 🇮🇹 Italian (Italiano)
  - 🇵🇹 Portuguese (Português)

---

### 11. 🛡️ Sovereign, Offline-First & Zero Ads
- **100% Offline Capability**: Once installed, no internet connection is required.
- **No Sign-Up Barrier**: Start working out in under 10 seconds without handing over email addresses or passwords.
- **No Telemetry, No Ad SDKs**: No trackers, no ad networks, no data brokers. Your fitness journey stays strictly yours.

---

## 🛠️ Technical Architecture

- **Language**: Kotlin 2.1
- **UI Framework**: Android Jetpack Compose (Material Design 3)
- **Computer Vision & On-Device AI**: Google MediaPipe Tasks Vision (`tasks-vision:0.10.14`)
- **Camera Subsystem**: AndroidX CameraX (Core, Camera2, Lifecycle, View)
- **Architecture**: Reactive MVVM with Kotlin Coroutines & `StateFlow`
- **Data Persistence**: Sovereign, typed JSON `LocalStore`
- **Design System**: Athletic dark palette `#0E1310`, tonal surfaces `#161C18` / `#1D2520`, electric lime accent `#C6F36A`.
- **Target Android**: `minSdk 26` (Android 8.0) • `targetSdk 36` (Android 16)

---

## ☕ Support the Project (Ko-fi & PayPal)

ATHLETIQ AI is created and maintained solo by **Sammy Yohan**. If this app helps your training and you want to give back to the project:

| Platform | Direct Link |
| :--- | :--- |
| ☕ **Ko-fi** | [ko-fi.com/sammyyohan](https://ko-fi.com/sammyyohan) |
| 💙 **PayPal** | [paypal.me/sammyyohan](https://paypal.me/sammyyohan) |

### What Donations Fund:
1. **Google Play Console Account Fee** ($25): To distribute ATHLETIQ AI directly on the Google Play Store for seamless automatic updates.
2. **A Second-Hand MacBook**: Necessary hardware to run macOS and Xcode, enabling the development and build of an iOS version.
3. **Apple Developer Program Fee** ($99/year): To publish and maintain the app on the Apple App Store.

---

## 📄 License & Rights

Designed and built with passion by **Sammy Yohan**.  
All rights reserved © 2026 Sammy Yohan.
