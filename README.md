# Coina - Cryptocurrency Mobile App

[![Kotlin](https://img.shields.io/badge/Kotlin-1.6.20-blue.svg)](https://kotlinlang.org/)
[![KMM](https://img.shields.io/badge/Kotlin%20Multiplatform-Mobile-green.svg)](https://kotlinlang.org/docs/multiplatform-mobile-overview.html)
[![Android](https://img.shields.io/badge/Android-API%2024+-brightgreen.svg)](https://developer.android.com/)
[![iOS](https://img.shields.io/badge/iOS-14.1+-lightgrey.svg)](https://developer.apple.com/ios/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

![](https://github.com/Yazan98/KMM-Cryptocurrency/blob/main/resources/app_landing_screen.png?raw=true)

> A modern cryptocurrency mobile application built with Kotlin Multiplatform Mobile (KMM) for Android and iOS platforms.

## 📱 Screenshots

| Android | iOS |
|---------|-----|
| ![](https://github.com/Yazan98/Coina/blob/main/resources/Screenshot%202022-12-30%20at%2010.32.59%20AM.png?raw=true) | ![](https://github.com/Yazan98/Coina/blob/main/resources/Screenshot%202022-12-30%20at%2011.29.07%20AM.png?raw=true) |

## 🚀 Description

**Coina** is a comprehensive cryptocurrency mobile application built using Kotlin Multiplatform Mobile (KMM) technology. The app provides real-time cryptocurrency information, market data, and portfolio tracking across both Android and iOS platforms with a shared codebase.

### Key Features
- **Cross-Platform**: Single codebase for Android and iOS
- **Real-time Data**: Live cryptocurrency prices and market information
- **Modern UI**: Material Design 3 on Android, SwiftUI on iOS
- **Offline Support**: Local data storage with Realm database
- **Dark/Light Theme**: Adaptive theming support
- **Modular Architecture**: Clean separation of concerns with feature modules

### Data Source
Powered by the free [CoinGecko API](https://www.coingecko.com/en/api/documentation) for real-time cryptocurrency data.

## 🏗️ Architecture

### Shared Module
The core of the application is built around a shared Kotlin module that contains:

- **Database Layer**: Realm database for local data persistence
- **API Layer**: HTTP client with Ktor for network requests
- **Storage Layer**: Cross-platform key-value storage (SharedPreferences/UserDefaults)
- **Business Logic**: Use cases and view models shared between platforms
- **Data Models**: Common data structures and serialization

### Platform-Specific Modules

#### Android Features
- `androidFeatures:core` - Core Android utilities and base classes
- `androidFeatures:auth` - Authentication screens and logic
- `androidFeatures:home` - Home screen and main navigation
- `androidFeatures:coin` - Cryptocurrency details and charts

## 📱 Application Features

### Core Screens
1. **Authentication Screen** - User login and session management
2. **Home Dashboard** - Market overview and trending cryptocurrencies
3. **Cryptocurrency List** - Comprehensive list of all available coins
4. **Exchange List** - Cryptocurrency exchange information
5. **Categories** - Cryptocurrency categories and classifications
6. **Category Coins** - Coins filtered by specific categories
7. **Coin Details** - Detailed information, charts, and market data

## 🛠️ Technology Stack

### Shared Module
- **Ktor Client** - HTTP networking and API communication
- **Realm Kotlin SDK** - Local database and data persistence
- **Kotlinx Serialization** - JSON serialization/deserialization
- **Kotlin Coroutines** - Asynchronous programming
- **CocoaPods** - iOS dependency management

### Android Platform
- **Jetpack Compose** - Modern declarative UI toolkit
- **Material Design 3** - Latest Material Design components
- **Hilt** - Dependency injection framework
- **Navigation Compose** - Type-safe navigation
- **Coil** - Image loading and caching
- **Firebase** - Analytics, Crashlytics, and cloud services
- **MPAndroidChart** - Interactive charts and graphs
- **Timber** - Logging framework
- **MultiDex** - Support for large applications

### iOS Platform
- **SwiftUI** - Declarative UI framework
- **Material Components** - Google's Material Design for iOS
- **ObjectMapper** - JSON object mapping
- **CocoaPods** - Dependency management
- **Ktor Darwin Client** - iOS-specific HTTP client

## 🎯 Learning Objectives

This project demonstrates several key concepts in mobile development:

1. **Cross-Platform Data Storage** - Shared key-value storage using SharedPreferences (Android) and UserDefaults (iOS)
2. **Shared ViewModels** - Business logic sharing between platforms with common state management
3. **Database Integration** - Realm database queries and local data persistence
4. **Navigation Patterns** - Platform-specific navigation implementations
5. **Theme Support** - Dark and light mode implementation across platforms
6. **Modular Architecture** - CocoaPods integration for shared library management

## 📊 Application Flow

### User Journey
![](https://github.com/Yazan98/Coina/blob/main/resources/User%20Flow.jpg?raw=true)

### Feature Architecture
![](https://github.com/Yazan98/Coina/blob/main/resources/Feature%20Flow.jpg?raw=true)

## 📸 Media Resources

- **Screenshots**: [View all application screenshots](https://github.com/Yazan98/Coina/tree/main/resources)
- **Demo Video**: [Platform comparison video](https://github.com/Yazan98/Coina/blob/main/resources/Compare%20Platforms.mp4)

## IDEs Requirements
1. Android Studio Version: Android Studio Flamingo | 2022.2.1 Canary 5
2. XCode Version: Version 14.2 (14C18)

## Steps to Run the Project
```
1. Open Android Studio with Root Application
2. Open Terminal and Execute (pod install)

If Gradle Build Failed for First Time
3. Execute Command (cd iosApp)
4. Execute Command (pod install)

5. Run The Android App
6. Open XCode with iosApp Folder
7. Execute Command (pod update shared)
8. Run IOS App
```

## Useful Resources

1. [Key Value Store](https://medium.com/@shmehdi01/shared-preference-in-kmm-kotlin-multiplatform-2bca14214093)
2. [SwiftUI](https://www.youtube.com/watch?v=TTYKL6CfbSs&list=PLwvDm4Vfkdphbc3bgy_LpLRQ9DDfFGcFu)
3. [Shared ViewModels](https://proandroiddev.com/kotlin-multiplatform-mobile-and-how-share-viewmodel-an-architecture-proposal-b6f86b61abf9)
4. [Shared ViewModels](https://medium.com/double-symmetry/kotlin-multiplatform-tales-a-shared-viewmodel-f9d0792f69f9)
5. [Ktor Documentation](https://ktor.io/docs/getting-started-ktor-client-multiplatform-mobile.html)
6. [KMM Documentation](https://kotlinlang.org/docs/multiplatform-mobile-ktor-sqldelight.html)
7. [Api Link](https://www.coingecko.com/en/api/documentation)
8. [Android Charts Library](https://github.com/PhilJay/MPAndroidChart)
9. [Realm Kotlin SDK](https://www.mongodb.com/docs/realm/sdk/kotlin/install/kotlin-multiplatform/)
10. [XCode-Kotlin Plugin](https://github.com/touchlab/xcode-kotlin)
