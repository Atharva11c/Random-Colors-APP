# 🎨 Random Colors iOS App

An iOS application that generates random colors, saves them locally, and syncs with Firebase Realtime Database when online. Built with SwiftUI, Core Data, and Firebase.

## ✨ Features

### 🎯 Core Functionality
- **Random Color Generation**: Generate beautiful random colors with a single tap
- **Color Display**: View colors in attractive cards with hex codes
- **Local Storage**: Save colors locally using Core Data for offline access
- **Persistent Data**: All saved colors persist between app launches

### 🌐 Firebase Integration
- **Real-time Sync**: Automatically syncs with Firebase Realtime Database when online
- **Offline Support**: Works seamlessly offline with automatic sync when connection is restored
- **Data Persistence**: Colors are stored with timestamps and device identification
- **Retry Mechanism**: Manual retry for failed sync operations

### 📱 User Experience
- **Network Awareness**: Real-time online/offline status indicator
- **Modern UI**: Clean, intuitive interface with smooth animations
- **Responsive Design**: Optimized for all iOS devices
- **Error Handling**: User-friendly error messages and crash prevention

### 🔧 Technical Features
- **SwiftUI**: Modern declarative UI framework
- **Core Data**: Robust local data persistence
- **Firebase**: Real-time cloud database integration
- **Network Monitoring**: Real-time connectivity detection
- **MVVM Architecture**: Clean separation of concerns

## 🚀 Getting Started

### Prerequisites
- Xcode 14.0 or later
- iOS 15.0 or later
- Firebase account
- iOS device or simulator

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Atharva11c/Random-Colors-APP.git
   cd Random-Colors-APP
   ```

2. **Open the project**
   ```bash
   open "Random Colors APP.xcodeproj"
   ```

3. **Firebase Setup**
   - Create a new Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Enable Realtime Database
   - Download `GoogleService-Info.plist` and add it to your project
   - The app is already configured to use Firebase Realtime Database

4. **Build and Run**
   - Select your target device or simulator
   - Press `Cmd + R` to build and run the app



## 🎨 How It Works

### Color Generation
1. Tap "Generate New Color" to create a random color
2. The color is displayed in a card with its hex code
3. Tap "Save" to store the color locally

### Data Storage
- **Local**: Colors are saved to Core Data for offline access
- **Cloud**: When online, colors automatically sync to Firebase
- **Sync Status**: Visual indicators show which colors are synced

### Network Handling
- **Online**: Automatic sync with Firebase Realtime Database
- **Offline**: Full functionality with local storage
- **Reconnection**: Automatic sync when network is restored

##  Configuration

### Firebase Setup
The app is pre-configured for Firebase Realtime Database. Ensure your `GoogleService-Info.plist` contains:

```xml
<key>DATABASE_URL</key>
<string>https://your-project.firebaseio.com</string>
```

### Core Data Model
The app uses a `SavedColor` entity with the following attributes:
- `hexCode`: Color hex value
- `timestamp`: When the color was saved
- `isSynced`: Sync status with Firebase
- `red`, `green`, `blue`: RGB components



### Main Screen
- Network status indicator
- Single color generation card
- Generate button
- Saved colors list
- Sync status and retry functionality

### Features
- **Network Status**: Green "Online" / Red "Offline" indicator
- **Color Cards**: Beautiful color display with hex codes
- **Save Functionality**: Individual save buttons for each color
- **Sync Indicators**: Visual feedback for sync status
- **Footer Stats**: App status and color count

##  Technologies Used

- **SwiftUI**: Modern iOS UI framework
- **Core Data**: Local data persistence
- **Firebase Realtime Database**: Cloud data storage
- **Combine**: Reactive programming framework
- **Network Framework**: Network connectivity monitoring


## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


