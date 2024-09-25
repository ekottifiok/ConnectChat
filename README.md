# ConnectChat

[GitHub][github]

[github]: https://github.com/ekottifiok/connect_chat

ConnectChat is a free, open-source app that allows you to securely share files and messages with nearby devices over your local network without needing an internet connection.

- [ConnectChat](#connectchat)
  - [About](#about)
  - [Screenshots](#screenshots)
    - [Desktop View](#desktop-view)
    - [Mobile View Dark Mode](#mobile-view-dark-mode)
  - [Download](#download)
  - [How It Works](#how-it-works)
  - [Getting Started](#getting-started)
  - [Building](#building)
    - [Android](#android)
    - [iOS](#ios)
    - [macOS](#macos)
    - [Windows](#windows)
    - [Linux](#linux)
  - [Contributing](#contributing)
    - [Translation](#translation)
    - [Bug Fixes and Improvements](#bug-fixes-and-improvements)
    - [Contributors](#contributors)

## About

ConnectChat is a cross-platform app that enables secure communication between devices using a REST API and HTTPS encryption. Unlike other messaging apps that rely on external servers, ConnectChat doesn't require an internet connection or third-party servers, making it a fast and reliable solution for local communication. It draws inspiration from WhatsApp to send messages, make calls both voice and video all without the internet

## Screenshots

### Desktop View

<img src="screenshots\Screenshot (124).png" />
<img src="screenshots\Screenshot (125).png" />
<img src="screenshots\Screenshot (126).png" />

### Mobile View Dark Mode

<img src="screenshots\Screenshot_20240325-203449.png" height="400" />
<img src="screenshots\Screenshot_20240325-203457.png" height="400" />
<img src="screenshots\Screenshot_20240325-203513.png" height="400" />
<img src="screenshots\Screenshot_20240325-203704.png" height="400" />

## Download

Right now this is in it devolopment phase, but once we done for a release we'll update this to show how you can download.

## How It Works

ConnectChat uses a secure communication protocol that allows devices to communicate with each other using a REST API. All data is sent securely over HTTPS, and the TLS/SSL certificate is generated on the fly on each device, ensuring maximum security.

For more information on the ConnectChat Protocol, see the [documentation](https://github.com/localsend/protocol).

## Getting Started

To compile ConnectChat from the source code, follow these steps:

1. Install [Flutter](https://flutter.dev).
2. Clone the ConnectChat repository.
3. Run `cd app` to enter the app directory.
4. Run `flutter pub get` to download dependencies.
5. Run `flutter run` to start the app.

The issue may be caused by a mismatch between the required Flutter version and the installed Flutter version.

ConnectChat uses [fvm](https://fvm.app) to manage the project Flutter version (specified in [app/.fvmrcn](app/.fvmrc)). After you install it, run `fvm flutter` instead of `flutter`.

## Building

These commands are intended for maintainers only.

### Android

Traditional APK

```bash
flutter build apk
```

AppBundle for Google Play

```bash
flutter build appbundle
```

### iOS

```bash
flutter build ipa
```

### macOS

```bash
flutter build macos
```

### Windows

**Traditional**

```bash
flutter build windows
```

**Local MSIX App**

```bash
flutter pub run msix:create
```

**Store ready**

```bash
flutter pub run msix:create --store
```

### Linux

**Traditional**

```bash
flutter build linux
```

**AppImage**

```bash
appimage-builder --recipe AppImageBuilder.yml
```

**Snap**

Feel free to open a pull request. There is a `snap` branch to play with.

## Contributing

We welcome contributions from anyone interested in helping improve ConnectChat. If you'd like to contribute, there are a few ways to get involved:

### Translation

You can help translate this app to other languages!

1. Fork this repository
2. Choose one
   - Add missing translations in existing languages: Only update `_missing_translations_<locale>.json` in [app/assets/i18n][i18n]
   - Fix existing translations: Update `strings_<locale>.i18n.json` in [app/assets/i18n][i18n]
   - Add new languages: Create a new file; see also: [locale codes][].
3. Optional: Re-run this app
   1. Run `cd app` to enter the app directory.
   2. Make sure you have [run](#getting-started) this app once.
   3. Update translations via `flutter pub run slang`
   4. Run the app via `flutter run`
   5. Open a pull request

[i18n]: https://github.com/ConnectChat/ConnectChat/tree/main/app/assets/i18n
[locale codes]: https://saimana.com/list-of-country-locale-code/

**_Take note:_ Fields decorated with `@` are not meant to be translated; they are not used in the app in any way, being merely informative text about the file or to give context to the translator.**

### Bug Fixes and Improvements

- **Bug Fixes:** If you find a bug, please create a pull request with a clear description of the issue and how to fix it.
- **Improvements:** Have an idea for how to improve LocalSend? Please create an issue first to discuss why the improvement is needed.

For more information, see the [contributing guide](https://github.com/ekottifiok/connect_chat/blob/main/CONTRIBUTING.md).

### Contributors

<a href="https://github.com/ekottifiok/connect_chat/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ekottifiok/connect_chat" />
</a>

Made with [contrib.rocks](https://contrib.rocks).
