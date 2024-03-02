# system_settings

Flutter plugin to open system and app settings from an iOS and Android app.

On **Android**, this plugin supports various system setting pages as well as the app info and app notification settings page.

On **iOS**, this plugin will always open the app settings page, if any settings have been defined via a `SettingsBundle`.
If not, the settings app will open with the home page. Unfortunately, this is the only way that complies with Apple's guidelines for the App Store.

## Getting Started

Add this to your package's pubspec.yaml file:

## FROM github

```yaml
dependencies:
  system_settings:
    git: https://github.com/AmirALMOHAMED/system_settings_plus.git
    ref: main
```
Alternatively, your editor might support dart pub get or flutter pub get. Check the docs for your editor to learn more.

Next, import the package into your dart code:

```dart
import 'package:system_settings/system_settings.dart';
```

## Example

Example which opens the app settings:

```dart
Widget build(BuildContext context) {
    return RaisedButton(
        onPressed: SystemSettings.app,
        child: Text('Open app settings'),
    );
}
```

## Bugs and feature requests

Have a bug or a feature request? Please first search for existing and closed issues.
If your problem or idea is not addressed yet, [please open a new issue](https://github.com/AmirALMOHAMED/system_settings_plus/issues).

