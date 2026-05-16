# 🚀 BCTransporter

**The Revolutionary Multi-Modal Transport Experience.**

BCTransporter is a premium, high-performance mobile application built with Flutter, designed to unify all transport needs—Buses, Trains, and Planes—into a single, stunning, and data-driven interface.

---

## 💎 Core Transport Modes

### 🚌 Bus Radar (Real-Time Tracking)
Don't just wait for the bus—watch it move. Our Bus module supports multiple providers with live GPS tracking and route visualization.
- **Multi-Provider Support**: Seamlessly switch between **Bari (AMTAB)**, **Emilia-Romagna (Tper)**, **Torino (GTT)**, and **Flixbus**.
- **Live Vehicle Positions**: Real-time updates on bus coordinates, heading, and speed.
- **Intelligent Stop Monitoring**: Get accurate arrival estimates and delay updates for every stop.
- **Route Pathing**: View the exact geographical path of your line directly on the map with polyline precision.

### 🚆 Train Hub (International Intelligence)
Navigate the rails with confidence across multiple countries and rail networks.
- **Global Station Coverage**: Real-time board for stations in **Italy, France, Germany, Switzerland, Austria**, and more.
- **Advanced Trip Details**: Full stop lists, scheduled vs. estimated times, platform changes, and status alerts.
- **FAL Integration**: Dedicated support for **Ferrovie Appulo Lucane (FAL)**, including specialized warnings and data feeds.
- **Interactive Rail Maps**: Visualize your train's journey with GeoJSON-powered polyline routes.

### ✈️ Flight Radar (Live Airspace)
Track the skies with a professional-grade flight radar integrated directly into your transport workflow.
- **Real-Time Flight Map**: Watch aircraft move in real-time with technical data (altitude, speed, heading, and squawk).
- **Airport Hub**: Search arrivals and departures for any airport globally by ICAO/IATA code.
- **Flight Analytics**: Access detailed flight info including airline, callsign, and estimated arrival windows.
- **Smooth Visuals**: High-performance rendering of airspace data with fluid map animations.

---

## 🛠️ Advanced Technologies

### 🔄 Intelligent Offline Sync
Never lose your route. BCTransporter features a robust **caching engine** that stores transport data locally.
- **Persistent Caching**: Works seamlessly on Mobile (Filesystem) and Web (SharedPreferences).
- **Auto-Sync**: Keeps your favorite lines and stations updated when connectivity is restored.
- **Metadata Tracking**: Monitor sync times and cache sizes for optimal performance.

### 🤖 Android Background Intelligence
Stay informed without even opening the app.
- **Native Background Workers**: Proactive monitoring of specific trips and stops.
- **Custom Notifications**: Get arrival notices (e.g., "5 minutes to arrival") via native Android notification channels.
- **Background Fetching**: Data is updated periodically even when the app is in the background.

### ☁️ Cloud & Security
- **Turso (LibSQL)**: Powered by a decentralized, edge-hosted database for fast and reliable user data sync.
- **Secure Auth**: Industry-standard **BCrypt** hashing for user security and session management.
- **Session Continuity**: Automatic session restoration across app restarts.

---

## ✨ Design Excellence
BCTransporter isn't just functional—it's beautiful.
- **Glassmorphism**: Modern UI components with translucent, blurred backgrounds for a premium feel.
- **Dynamic Themes**: Full support for sleek Dark and Light modes.
- **Micro-Animations**: Smooth transitions and interactive elements that make the app feel alive.
- **Map Centricity**: A focus on geographic visualization to make transport intuitive.

---

## 🚀 Getting Started

### Credits

We would like to express our gratitude to Martin ([[@CuzImMartin|Thanks to [[Martin|https://github.com/CuzImMartin]] to grent me access to his api for train services) for providing access to his proprietary API for train services.

### Prerequisites
- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- [Dart SDK](https://dart.dev/get-started)

---

*Designed and Developed with ❤️ for the future of mobility.*
