# 🐦 Birdie
 
A delightful macOS menu bar app that sends an animated bird flying across your screen to remind you about upcoming Google Calendar events.
 
---
 
## ✨ Features
 
- **Animated bird notifications** — a cute bird flies across your screen before meetings start
- **Google Calendar integration** — connects to your primary calendar via Google Sign-In
- **Smart reminders** — alerts you up to 5 minutes before an event
- **Non-intrusive** — lives quietly in your menu bar until it's time to remind you
- **Pause on hover** — hover over the bird to pause it mid-flight
---
 
## 📸 Preview
 
> A bird flies across your screen carrying your meeting name — hard to miss, impossible to hate.
 
---
 
## 🚀 Getting Started
 
### Prerequisites
 
- macOS 13+
- Xcode 15+
- A Google account with Calendar access
### Installation
 
1. Clone the repo
   ```bash
   git clone https://github.com/kavyakunder/Birdie.git
   cd Birdie
   ```
 
2. Create a `Secrets.xcconfig` file in the project root (not tracked by git):
   ```
   GOOGLE_CLIENT_ID = your-google-client-id-here
   ```
 
3. Open `Reminderapp.xcodeproj` in Xcode
4. Build and run (`Cmd + R`)
### Google Calendar Setup
 
1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a project and enable the **Google Calendar API**
3. Create an **OAuth 2.0 Client ID** (macOS app)
4. Add the client ID to your `Secrets.xcconfig`
---
 
## 🛠 Tech Stack
 
- **SwiftUI** — UI and animations
- **Google Sign-In SDK** — OAuth authentication
- **Google Calendar REST API** — fetching events
- **GIF rendering** — custom `GifView` for the animated bird
---
 
## 📁 Project Structure
 
```
Birdie/
├── ReminderappApp.swift      # App entry, menu bar setup
├── AuthManager.swift         # Google Sign-In + Calendar API
├── BirdOverlay.swift         # Overlay window management
├── BirdView.swift            # Animated bird + message UI
├── GifView.swift             # GIF rendering
└── Assets/                   # App icons and GIF assets
```
 
---
 
## 🔒 Security
 
- OAuth credentials are stored in `Secrets.xcconfig` which is gitignored
- No credentials are hardcoded or committed to the repository
---
 
## 🧡 Made by
 
[Kavya Kunder](https://github.com/kavyakunder) — built with SwiftUI and too many test calendar meetings.
 
