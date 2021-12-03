# Screen

A Flutter plugin to manage the device's screen on Android and iOS.

This is a fork from [Screen](https://github.com/clovisnicolas/flutter_screen) with Null Safety support added.

## Usage

To use this plugin, add the dependency on your pubspec:

```
  screen:
    git:
      url: https://github.com/daniloapr/flutter_screen.git
```

Make sure you add the following permissions to your Android Manifest

```
<uses-permission android:name="android.permission.WAKE_LOCK" />
```

## Example

```dart
// Import package
import 'package:screen/screen.dart';

// Get the current brightness:
double? brightness = await Screen.brightness;

// Set the brightness:
Screen.setBrightness(0.5);

// Check if the screen is kept on:
bool? isKeptOn = await Screen.isKeptOn;

// Prevent screen from going into sleep mode:
Screen.keepOn(true);
```
