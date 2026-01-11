# QuickTask Pro

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Flutter](https://img.shields.io/badge/Flutter-v3.0+-02569B.svg)
![Dart](https://img.shields.io/badge/Dart-v3.0+-0175C2.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

QuickTask Pro is a sophisticated task management application architected with **Flutter** and **Dart**, powered by **Back4App** (Parse Server) for a scalable and secure backend. This project serves as a comprehensive demonstration of full-stack mobile development, featuring real-time data synchronization, user session management, and CRUD operations.

## 🌟 Key Features

### 🔐 Robust Authentication
*   **Secure Sign Up & Log In**: Implements ParseUser for handling secure registration and authentication.
*   **Session Persistence**: Automatic session management ensures users stay logged in across app restarts.

### 📝 Comprehensive Task Management
*   **Create**: Add tasks with title and precise due dates.
*   **Read**: Real-time fetching of user-specific tasks.
*   **Update**: Modify task details including title and due date.
*   **Delete**: Remove tasks permanently from the database.
*   **Toggle Status**: Mark tasks as "Completed" or "Pending" with instant visual feedback.

### 🎨 Modern UI/UX
*   **Material Design**: Follows Material 3 guidelines for a clean, modern aesthetic.
*   **Responsive Layouts**: Optimized for various screen sizes.

## 🛠 Tech Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Frontend** | Flutter (Dart) | Cross-platform UI framework. |
| **Backend** | Back4App | Backend-as-a-Service (BaaS) based on Parse Platform. |
| **Database** | MongoDB | NoSQL database managed by Back4App. |
| **CI/CD** | GitHub Actions | Automated build pipeline for Android APKs. |

## � Installation & Setup

### Prerequisites
*   [Flutter SDK](https://docs.flutter.dev/get-started/install) (Stable channel)
*   [Android Studio](https://developer.android.com/studio) or VS Code
*   [Git](https://git-scm.com/)

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/QuickTask_Pro.git
cd QuickTask_Pro
```

### 2. Backend Configuration (Back4App)
1.  Create an account at [Back4App](https://www.back4app.com/).
2.  Create a new App named `QuickTask Pro`.
3.  Go to **App Settings > Security & Keys**.
4.  Copy your `Application ID` and `Client Key`.
5.  Open `lib/main.dart` (or your constants file) and update the credentials:
    ```dart
    const keyApplicationId = 'YOUR_APP_ID_HERE';
    const keyClientKey = 'YOUR_CLIENT_KEY_HERE';
    ```

### 3. Install Dependencies
```bash
flutter pub get
```

### 4. Run the Application
```bash
flutter run
```

## 🏗 Project Structure

```
lib/
├── main.dart           # Entry point and app initialization
├── screens/            # UI screens (Login, Home, TaskDetail)
├── models/             # Data models (Task, User)
├── services/           # Backend services (AuthService, TaskService)
├── widgets/            # Reusable UI components
└── utils/              # Helper functions and constants
```

## 📸 Screenshots

| Login Screen | specific Task List | Task Details |
| :---: | :---: | :---: |
| ![Login](https://via.placeholder.com/150x300?text=Login) | ![List](https://via.placeholder.com/150x300?text=List) | ![Details](https://via.placeholder.com/150x300?text=Details) |

## ❓ Troubleshooting

**Issue: "Client not initialized"**
*   *Fix*: Ensure `Parse().initialize()` is called in `main.dart` before `runApp()`.

**Issue: Build failures on Android**
*   *Fix*: Check `android/build.gradle` for compatible Kotlin version and ensure `minSdkVersion` is at least 21.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:
1.  Fork the project.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
