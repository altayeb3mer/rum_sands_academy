
# Rum Sands Academy Flutter App

This is the official Flutter app for Rum Sands Academy. It launches a web view to the academy's website and supports localization for English and Arabic.

## Features

- WebView for https://rumsands.com
- Localized app name and UI (English & Arabic)
- Custom app icon (see `assets/images/rum_logo.jpeg`)
- Navigation controls (back, forward, refresh)

## Localization

Localization is implemented using Flutter's `flutter_localizations` and `intl` packages.

- ARB files for strings: `lib/l10n/app_en.arb` (English), `lib/l10n/app_ar.arb` (Arabic)
- To add or update translations:
  1. Edit the ARB files in `lib/l10n/`.
  2. Run `flutter gen-l10n` to regenerate localization code.
  3. Use `AppLocalizations.of(context)!.yourKey` in your widgets.

## App Icon

The app icon is generated from `assets/images/rum_logo.jpeg` using the `flutter_launcher_icons` package.

To update the icon:
1. Replace the image at `assets/images/rum_logo.jpeg`.
2. Run `flutter pub run flutter_launcher_icons:main`.

## How to Update

- **Dependencies:** Run `flutter pub get` after changing `pubspec.yaml`.
- **Localization:** Edit ARB files and run `flutter gen-l10n`.
- **App Icon:** Update logo and run launcher icons command.
- **Push to GitHub:**
  1. `git add .`
  2. `git commit -m "your message"`
  3. `git push`

## Developer Notes

- Supports Android, iOS, Web, macOS, Windows, Linux.
- Main entry: `lib/main.dart`
- WebView widget: `lib/webview_screen.dart`
- App name is localized and set in both ARB files and platform configs (AndroidManifest.xml, Info.plist).

## Resources

- [Flutter Localization Docs](https://docs.flutter.dev/development/accessibility-and-localization/internationalization)
- [flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons)

---
For help getting started with Flutter development, view the [online documentation](https://docs.flutter.dev/), which offers tutorials, samples, guidance on mobile development, and a full API reference.
