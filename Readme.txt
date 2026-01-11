QuickTask Pro
=============
Version: 1.2
License: MIT

QuickTask Pro is a sophisticated task management application built with Flutter and Dart, utilizing Back4App (Parse Platform) for its backend. It demonstrates full-stack mobile development with real-time features.

KEY FEATURES
------------
1. Authentication:
   - Secure Sign Up/Log In via ParseUser.
   - Persistent sessions.

2. Task Management:
   - CRUD operations (Create, Read, Update, Delete).
   - Real-time data synchronization.
   - Status toggling (Completed/Pending).

3. Technical Stack:
   - Frontend: Flutter (Dart)
   - Backend: Back4App (Parse/MongoDB)
   - Automation: GitHub Actions (CI/CD)

SETUP INSTRUCTIONS
------------------
1. Install Flutter SDK and Git.
2. Clone the repo: `git clone https://github.com/your-username/QuickTask_Pro.git`
3. Setup Back4App:
   - Create an app on Back4App.
   - Get `Application ID` and `Client Key` from App Settings.
   - Update credentials in `lib/main.dart`.
4. Run `flutter pub get`.
5. Run `flutter run`.

TROUBLESHOOTING
---------------
- If you see "Client not initialized", check your Back4App keys in `main.dart`.
- Ensure Android `minSdkVersion` is set to 21 or higher.

For full documentation and screenshots, please refer to the README.md file.