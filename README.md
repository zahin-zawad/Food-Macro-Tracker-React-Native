# Food Macro Tracker

Food Macro Tracker is a simple Expo-based mobile app for logging meals and tracking daily nutrition goals. It helps you quickly record calories, protein, carbs, and fat, then review your recent meals from the home screen.

## Features

- Add meals with calories and macronutrients
- View a daily macro summary on the home screen
- Review recent meals and delete entries
- Copy or share a daily summary
- Optional meal reminders (on supported devices)
- Local persistence using AsyncStorage

## Requirements

- Node.js 18+
- npm or yarn
- Expo CLI
- Android Studio / Xcode (optional, for running on emulators/simulators)

## Installation

1. Clone the repository
   ```bash
   git clone https://github.com/zahin-zawad/Food-Macro-Tracker-React-Native.git
   cd food-macro-tracker
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. If you run into icon-related errors, install the icon package:
   ```bash
   npx expo install @expo/vector-icons
   ```

## Running the app

Start the Expo development server:

```bash
npx expo start
```

Then choose one of the following:
- Press `i` to open the iOS simulator
- Press `a` to open the Android emulator
- Scan the QR code in Expo Go on your phone
- Press `w` to open the web version

## How to use it

1. Open the app on your device or emulator.
2. On the home screen, you will see your daily macro summary and recent meals.
3. Tap the add-meal tab to log a new meal.
4. Enter the meal name and nutrition values, then tap Add Meal.
5. Your meal will appear in the recent list and contribute to the summary.
6. Use the share button to send a daily summary, or enable meal reminders from the home screen.

## Project structure

- `src/app` - Expo Router screens and tab navigation
- `src/components` - Reusable UI components
- `src/storage` - Local meal storage using AsyncStorage
- `src/styles` - Shared styling and theme values
- `src/utils` - Notification helpers

## Notes

- Meal data is stored locally on the device, so it will persist between app launches.
- Reminder permissions may be required before enabling notifications.
- For a clean reload after changing app configuration, you can run:

```bash
npx expo start --clear
```
