# Contributing to AnimeStream

Thank you for your interest in contributing to AnimeStream! This document provides detailed guidelines, especially for developers looking to set up the project and make code contributions.

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Development Setup](#development-setup)
  - [Prerequisites](#prerequisites)
  - [Getting the Code](#getting-the-code)
  - [Installing Dependencies](#installing-dependencies)
  - [Running the App](#running-the-app)
- [Project Structure](#project-structure)
- [Development Workflow](#development-workflow)
  - [Creating a Branch](#creating-a-branch)
  - [Writing Code](#writing-code)
  - [Testing](#testing)
  - [Building for Release](#building-for-release)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Style Guides](#style-guides)

## Code of Conduct

This project adheres to the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/). By participating, you are expected to uphold this code.

## How to Contribute

You can contribute by:
- Reporting bugs
- Suggesting new features
- Writing or improving documentation
- Fixing bugs or implementing new features (see the development section below)

## Development Setup

This section will guide you through the process of setting up the AnimeStream project on your local machine for development.

### Prerequisites

Before you begin, ensure you have the following installed:
- **Git**: For version control.
- **Flutter SDK**: The project is built with Flutter. You can install it by following the official [Flutter installation guide](https://docs.flutter.dev/get-started/install). Make sure to also install the necessary platform-specific dependencies (Android SDK for Android development, Xcode for iOS, etc.).
- **A code editor**: [Visual Studio Code](https://code.visualstudio.com/) with the Flutter extension or [Android Studio](https://developer.android.com/studio) are recommended.

### Getting the Code

1.  Fork the repository on GitHub.
2.  Clone your fork to your local machine:
    ```bash
    git clone https://github.com/YOUR-USERNAME/animestream.git
    cd animestream
    ```
3.  Add the original repository as an upstream remote to keep your fork updated:
    ```bash
    git remote add upstream https://github.com/frostnova721/animestream.git
    ```

### Installing Dependencies

The project's dependencies are managed in the `pubspec.yaml` file, which is standard for all Flutter applications . To install them:

1.  Navigate to the project's root directory (where `pubspec.yaml` is located).
2.  Run the following command:
    ```bash
    flutter pub get
    ```
    This command will download and install all the packages listed in the `pubspec.yaml` file .

### Running the App

Once the dependencies are installed, you can run the app on an emulator, simulator, or a physical device connected to your machine.

- **For development (debug mode)**:
    ```bash
    flutter run
    ```
    This will build and launch the app in debug mode, which includes useful debugging tools.

## Project Structure

While the exact internal structure of the `frostnova721/animestream` repository isn't publicly detailed in the search results, it is a standard Flutter application . A common and scalable structure for such apps often follows a layered architecture to separate concerns:

```
animestream/
├── lib/
│   ├── main.dart                 # The main entry point of the app.
│   ├── models/                   # Data models (e.g., Anime, Episode).
│   ├── services/                 # Business logic and API clients.
│   │   └── api_service.dart
│   ├── repositories/             # Data layer that abstracts data sources.
│   ├── screens/                  # Top-level screen widgets.
│   │   └── home_screen.dart
│   └── widgets/                  # Reusable UI components.
│       └── anime_card.dart
├── assets/                       # Static assets like images, fonts, etc.
├── pubspec.yaml                  # Project metadata and dependencies.
└── ...
```
This structure helps keep the code organized, testable, and maintainable as the project grows .

## Development Workflow

### Creating a Branch

For any new feature or bug fix, create a new branch from the `main` branch of the upstream repository.

```bash
# Fetch the latest changes from upstream
git fetch upstream
# Create a new branch based on the updated main
git checkout -b your-branch-name upstream/main
```

### Writing Code

- **Follow the Style Guide**: Adhere to the [Effective Dart: Style](https://dart.dev/guides/language/effective-dart/style) guide. Use `dart format` to automatically format your code before committing.
- **Write Clear Code**: Use descriptive names for variables, functions, and classes. Add comments where necessary to explain complex logic.
- **Handle State and Data**: If you are adding new features that fetch data, integrate them with the existing service/repository pattern if one exists.

### Testing

While the project's current testing strategy isn't specified, it's good practice to:
- Manually test your changes on different screen sizes and platforms.
- If the project has unit or widget tests, add new tests for your code or update existing ones. Run tests with `flutter test`.

### Building for Release

Once your feature is complete and tested, you might want to build a release version of the app to test its performance or for distribution.

- **To build an Android APK**:
    ```bash
    flutter build apk
    ```
    The APK will be located in `build/app/outputs/flutter-apk/` .

- **For a more optimized build** (splits APK by CPU architecture):
    ```bash
    flutter build apk --split-per-abi
    ```

## Pull Request Guidelines

1.  **Squash your commits**: Before submitting your PR, please squash your commits into a single, logical commit with a clear message.
2.  **Update your branch**: Ensure your branch is up-to-date with the `main` branch of the upstream repository to avoid merge conflicts.
3.  **Fill out the PR template**: Provide a clear description of the problem you're solving and the changes you've made. Link to any related issues.
4.  **Verify checks**: After you submit your PR, ensure all automated checks (like CI builds) are passing.

## Style Guides

- **Dart**: Follow the [Effective Dart: Style](https://dart.dev/guides/language/effective-dart/style) guide.
- **Flutter**: Adhere to common Flutter best practices for widget composition and state management.
