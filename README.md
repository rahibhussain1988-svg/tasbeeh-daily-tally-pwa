# 📿 Tasbeeh & Daily Tally Counter (PWA)

> **Touch-Optimized Islamic Tasbeeh, Multi-Counter & Daily Tally Progressive Web App (PWA) with 100% Offline Storage, Web Audio & Haptic Feedback.**

[![PWA Ready](https://img.shields.io/badge/PWA-Installable-059669?style=flat-square&logo=pwa)](https://github.com/rahibhussain1988-svg/tasbeeh-daily-tally-pwa)
[![Offline Ready](https://img.shields.io/badge/Offline-100%25%20Cache-teal?style=flat-square)](https://github.com/rahibhussain1988-svg/tasbeeh-daily-tally-pwa)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Deployment-GitHub%20Pages-0284c7?style=flat-square&logo=github)](https://rahibhussain1988-svg.github.io/tasbeeh-daily-tally-pwa/)

---

## 📱 Live Demo & Deployment

* **Live GitHub Pages Web App**: [https://rahibhussain1988-svg.github.io/tasbeeh-daily-tally-pwa/](https://rahibhussain1988-svg.github.io/tasbeeh-daily-tally-pwa/)
* **Repository**: [https://github.com/rahibhussain1988-svg/tasbeeh-daily-tally-pwa](https://github.com/rahibhussain1988-svg/tasbeeh-daily-tally-pwa)

---

## 🌟 Key Features

### 1. 🔘 Ergonomic Giant Circular Touch Zone
- **Thumb-Friendly Tactile Counting**: Full touch area designed for one-handed operation on mobile devices.
- **Double-Tap & Zoom Prevention**: Built-in touch listeners prevent accidental zoom and browser ghost clicks.
- **Dynamic Circular Progress Ring**: SVG stroke progress circle visually tracks progress towards the counter's target goal.
- **Micro-Animations**: Elastic number pop effect and touch-anchored radial ripples.
- **Keyboard Navigation**: Press <kbd>Space</kbd> or <kbd>Arrow Up</kbd> to increment on desktop.

### 2. 📿 Built-in Dhikr Presets & Custom Counters
Includes pre-configured Islamic Dhikr counters with authentic Arabic text and targets:
- **سُبْحَانَ اللَّهِ (SubhanAllah)** — Target: 33
- **الْحَمْدُ لِلَّهِ (Alhamdulillah)** — Target: 33
- **اللَّهُ أَكْبَرُ (Allahu Akbar)** — Target: 34
- **أَسْتَغْفِرُ اللَّهَ (Astaghfirullah)** — Target: 100
- **Daily Tally** — General multi-purpose count (Unlimited)
- **Unlimited Custom Counters**: Create any custom counter with custom step increments (+1, +5, etc.), target presets (33, 99, 100, 500, 1000, or unlimited), and 6 accent colors (Emerald, Teal, Sky, Violet, Amber, Rose).

### 3. 📊 Daily Tally & Activity Screen
- **Direct Value Addition**: Add batches (e.g. `+50`, `+120`, `-15`) with optional timestamped notes.
- **1-Tap Quick Adder Chips**: Instant `+1`, `+5`, `+10`, `+50`, and `+100` chips.
- **Per-Counter Breakdown**: Displays daily grand totals and per-counter breakdowns for today, yesterday, and any prior date.
- **Timestamped Activity Log with Undo**: View recent activity log entries with 1-tap **Undo Last** action.

### 4. 🔊 Real-Time Audio & Haptic Feedback
- **Web Audio API Sound Synthesizer**: Generates organic wooden bead clicks without relying on external MP3 files.
- **Harmonic Target Chime**: Two-note sine chord (523.25 Hz & 659.25 Hz) rings when the target cycle completes.
- **Haptic Vibration**: Native Android `navigator.vibrate` delivers tactile click feedback and distinct multi-pulse vibration on cycle completion.
- **Toggle Controls**: 1-click sound and vibration mute buttons directly in the top app header.

### 5. 🌓 Dark / Light Theme & Responsive Design
- Modern Tailwind CSS dark/light theme switcher with automatic state memory.
- Mobile full-bleed safe area padding (`env(safe-area-inset-bottom)`) tailored for notched Android & iOS screens.
- Desktop and tablet centered layout with subtle elevation and backdrop blur effects.

### 6. 💾 100% Local Storage & JSON Backup / Restore
- **Privacy-First**: No tracking, no external database, no accounts required. All data stays on the user's device.
- **JSON Export**: Export full counter history, daily totals, and logs as a `.json` backup file.
- **JSON Import**: Easily restore or transfer your counts across devices.

### 7. 📲 Progressive Web App (PWA) Offline Installation
- Complete `manifest.json` with vector and maskable icons.
- Service Worker (`sw.js`) with cache-first strategy for instant offline loading anywhere, anytime.

---

## 📁 Project Structure

```
tasbeeh-daily-tally-pwa/
├── index.html                           # Main PWA application entry point
├── manifest.json                        # PWA Web App Manifest
├── sw.js                                # Offline Service Worker cache engine
├── favicon.svg                          # Browser tab icon
├── icons/
│   ├── icon.svg                         # Master high-resolution 512x512 vector icon
│   ├── icon-192.svg                     # 192x192 PWA icon
│   ├── icon-512.svg                     # 512x512 PWA icon
│   └── icon-maskable.svg                # Android maskable icon
├── tasbeeh_daily_tally_counter_pwa.html # Standalone self-contained single-file build
├── .gitignore                           # Git ignore rules
└── README.md                            # Documentation & installation guide
```

---

## 🚀 How to Run Locally

### Option 1: Direct File Opening
Double-click `index.html` or `tasbeeh_daily_tally_counter_pwa.html` to open in any web browser.

### Option 2: Local HTTP Server (Recommended for PWA testing)
Using Node.js:
```bash
npx serve .
# or
npx http-server -p 8080
```
Using Python 3:
```bash
python -m http.server 8080
```
Open [http://localhost:8080](http://localhost:8080) in Google Chrome or Microsoft Edge.

---

## 📲 How to Install as an App

### On Android (Google Chrome / Brave / Edge)
1. Open the app link in **Chrome** on your phone.
2. Tap the **Install** button in the top header, or tap the three dots **(⋮)** in the top right.
3. Select **"Add to Home screen"** or **"Install app"**.
4. The app icon will appear on your home screen and open in full-screen standalone mode.

### On iOS (Apple Safari)
1. Open the app link in **Safari**.
2. Tap the **Share** button (box with an upward arrow).
3. Scroll down and tap **"Add to Home Screen"**.

### On Desktop (Chrome / Edge)
1. Click the **Install** icon in the browser address bar.
2. Launch directly from your desktop or start menu.

---

## 🛠️ Technology Stack

- **HTML5 & Vanilla JavaScript**: High performance, zero runtime overhead.
- **Tailwind CSS**: Utility-first responsive styling with dark mode support.
- **Web Audio API**: Real-time sound synthesis for bead clicks and harmonic chimes.
- **Vibration API**: Native hardware haptics for touch feedback.
- **Web App Manifest & Service Worker**: Full PWA offline capability.
- **LocalStorage API**: Reliable, instant on-device data persistence.

---

## 👤 Author & Repository

- **Author**: Rahib Hussain ([@rahibhussain1988-svg](https://github.com/rahibhussain1988-svg))
- **Repository**: [https://github.com/rahibhussain1988-svg/tasbeeh-daily-tally-pwa](https://github.com/rahibhussain1988-svg/tasbeeh-daily-tally-pwa)
- **License**: MIT
