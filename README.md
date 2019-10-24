# Gatekeeper Native Swiper

This is a project with a test component to do a swipeable effect between components.

- [Gatekeeper Native Swiper](#gatekeeper-native-swiper)
  - [Installation](#installation)
    - [To run iOS](#to-run-ios)
    - [To run Android](#to-run-android)

## Installation

First thing you need to have in your OSMac is:

1. Node
2. Watchman
   1. For Watchman, is recommended to be installed with **Brew**

`brew install watchman`

After installing the necessary dependencies, is important to run some commands before trying to run the project.</br>
First of all:

```bash
yarn
```

Once installed all dependencies.

### To run iOS

Inside the folder ios

```bash
cd ios/
pod install
cd ..
```

Now, inside your project folder in the Terminal:

`react-native run-ios --verbose`

### To run Android

Inside the folder android/app

```bash
cd android/app
keytool -genkey -v -keystore debug.keystore -storepass android -alias androiddebugkey -keypass android -keyalg RSA -keysize 2048 -validity 10000
# Follow the prompts and once finished
cd ../..
```

> ☝️ This solution was extrated from here [Task :app:validateSigningDebug FAILED ✅ SOLUTION](https://stackoverflow.com/a/57104505)

Now, inside your project folder in the Terminal:

`react-native run-android --verbose`
