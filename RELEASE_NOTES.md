# Release Notes - v1.3

## 🚀 Overview
QuickTask Pro v1.3 focuses on stabilizing the CI/CD pipeline and modernizing the build configuration.

## ✨ New Features & Improvements
*   **Android Build Action**: Fixed path issues in GitHub Actions to correctly build the APK from the `QuickTask_app` directory.
*   **Gradle Migration**: Migrated to the new declarative Flutter Gradle Plugin, resolving deprecated `apply script` warnings.
*   **Artifact Cleanup**: implementing a cleaner `.gitignore` to prevent build artifacts from polluting the repository.

## 🐛 Bug Fixes
*   Fixed `URISyntaxException` in CI builds caused by hardcoded Windows paths in committed build files.
*   Resolved `actions/upload-artifact` deprecation warnings by upgrading to v4.

## 📦 Build Details
*   **Version**: 1.3.0
*   **Build Number**: 13
*   **Engine**: Flutter 3.19.0
