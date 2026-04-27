# Parallel Connect

An immersive Android mobile application that simulates a mystical world where users can discover, interact with, and communicate with ghosts and spirits through location-based exploration and AI-powered conversations.

## 🎯 Overview

Parallel Connect is a unique mobile experience that combines location-based gaming with artificial intelligence to create an engaging supernatural world. Users explore their real-world surroundings to find spirits, capture photographic evidence, and engage in meaningful conversations with AI-powered ghost characters, each with their own backstory and personality.

## ✨ Key Features

### 🗺️ **Location-Based Spirit Discovery**
- Real-time GPS tracking to locate spirits in your vicinity
- Interactive map with custom spirit markers
- Proximity-based spirit encounters
- Location-specific spirit spawning system

### 👻 **Interactive Spirit Characters**
- **Jeff**: A spirit who died while changing a car lamp
- **Martin**: A cheerful spirit who found happiness in the afterlife
- **Sarah**: A mother spirit who sacrificed herself for her children
- Each spirit has unique personalities and backstories

### 💬 **AI-Powered Conversations**
- Real-time chat with discovered spirits using Google Gemini AI
- Persistent conversation history stored in Firebase
- Contextual responses based on each spirit's character profile
- Real-time message synchronization across devices

### 📸 **Evidence Collection System**
- In-app camera functionality for capturing paranormal evidence
- Photo gallery for storing and managing captured images
- Firebase integration for cloud storage of evidence
- Timestamp and location metadata for each photo

### 🔐 **User Authentication & Profiles**
- Secure Firebase Authentication system
- User profile management
- Personalized spirit collection tracking
- Conversation history persistence

## 🏗️ Architecture

### **Technology Stack**
- **Frontend**: Android Jetpack Compose (Kotlin)
- **Backend**: Firebase Realtime Database & Authentication
- **AI**: Google Gemini 1.5 Flash API
- **Maps**: Google Maps API with Android Maps Utils
- **Location**: Google Play Services Location API
- **Architecture**: MVVM (Model-View-ViewModel) pattern

### **Core Components**
- **Navigation**: Jetpack Navigation Compose
- **State Management**: ViewModel with Compose State
- **Real-time Data**: Firebase Realtime Database listeners
- **AI Integration**: Google Generative AI SDK
- **Location Services**: FusedLocationProviderClient

## 📱 App Flow

1. **Authentication**: Users login or register
2. **Main Menu**: Access to map and conversation features
3. **Spirit Discovery**: Open map to find nearby spirits
4. **Spirit Interaction**: Tap markers to discover and chat with spirits
5. **Evidence Collection**: Take photos of paranormal activity
6. **Gallery Management**: View and organize captured evidence

## 🗂️ Project Structure

```
app/src/main/java/com/example/parallel_connect/
├── MainActivity.kt                 # Main activity entry point
├── screens/                       # UI screens
│   ├── MainActivity.kt
│   ├── MainMenu.kt
│   ├── MapScreen.kt
│   ├── SpiritFoundScreen.kt
│   ├── LoginScreen.kt
│   ├── RegistrationScreen.kt
│   ├── ProfileScreen.kt
│   ├── ConversationsListScreen.kt
│   ├── JeffChat.kt
│   ├── MartinChat.kt
│   ├── SarahChat.kt
│   ├── PhotoGalleryScreen.kt
│   ├── ForumShoesScreen.kt
│   ├── NavGraph.kt
│   └── Screens.kt
├── viewModels/                    # MVVM ViewModels
│   ├── JeffChatViewModel.kt
│   ├── MartinChatViewModel.kt
│   └── SarahChatViewModel.kt
└── ui/theme/                      # App theming
    ├── Color.kt
    ├── Theme.kt
    └── Type.kt
```

## 🚀 Getting Started

### **Prerequisites**
- Android Studio Hedgehog | 2023.1.1 or later
- Kotlin 1.9.0+
- Android SDK API 24+ (Android 7.0)
- Google Play Services

### **How to Run**

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Parallel-Connect.git
   cd Parallel-Connect
   ```



2. **Open in Android Studio**
   - Open Android Studio
   - Select "Open an existing project"
   - Navigate to the cloned repository folder

3. **Build and Run**
   Run the app directly from Android Studio using the green play button.

   Or

   Run the apk


## 🎮 Usage Guide

### **Finding Spirits**
1. Grant location permissions when prompted
2. Navigate to the Map screen from the main menu
3. Look for ghost markers near your location
4. Tap on markers to discover spirits

### **Chatting with Spirits**
1. After discovering a spirit, choose to talk with them
2. Type messages in the chat interface
3. Receive AI-powered responses based on the spirit's personality
4. Conversation history is automatically saved

### **Taking Photos**
1. Use the camera button on the map screen
2. Capture evidence of paranormal activity
3. Save photos to your personal gallery
4. Access photos through the menu dropdown

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Development Notes

### **AI Integration**
- Each spirit uses Google Gemini 1.5 Flash with custom prompts
- Responses are generated in real-time based on user input
- Conversation context is maintained through Firebase

### **Location Services**
- Uses FusedLocationProviderClient for accurate GPS data
- Spirits spawn within ~100 meters of user location
- Camera automatically focuses on user's position

### **Performance Considerations**
- LazyColumn used for efficient chat message rendering
- Firebase listeners are properly managed to prevent memory leaks
- Image loading optimized with Coil library

## 🐛 Known Issues

- Spirit markers may not update immediately after location changes
- Camera permissions need to be manually granted on some devices
- AI responses may have latency depending on network conditions


## 🙏 Acknowledgments

- **Google** - Gemini AI API and Maps Platform
- **Firebase** - Authentication and Realtime Database
- **Jetpack Compose** - Modern UI toolkit
- **Android Maps Utils** - Map utilities and markers

## 📞 Contact

For questions, suggestions, or issues, please open an issue on GitHub.

---

**Parallel Connect** - Where the spirit world meets technology 🌟
