<p align="center">
  <h1 align="center">VEDAgram</h1>
  <p align="center">Custom Telegram client for Android</p>
</p>

VEDAgram is a custom Telegram client for Android based on [Finegram](https://github.com/Th3Nekit/Finegram), [Cherrygram](https://github.com/arsLan4k1390/Cherrygram), and [Telegram for Android](https://github.com/DrKLO/Telegram).

It keeps the powerful Finegram foundation while using its own VEDAgram identity and application package.

## Features

- Telegram messaging on Android
- Built-in anti-censorship and proxy features inherited from Finegram
- Plugin support
- Privacy-oriented options
- Extensive interface customization
- Custom VEDAgram application ID: `com.vedagram.app`

## Build

Requirements: JDK 17, Android SDK 36, Build Tools 36.0.0, NDK 27.2.12479018, CMake 3.22.1, and Python 3.11.

Create `private.properties` in the repository root:

```properties
TELEGRAM_API_ID=your_api_id
TELEGRAM_API_HASH=your_api_hash
KEYSTORE_PATH=path/to/your.jks
KEYSTORE_PASSWORD=your_password
KEY_ALIAS=your_alias
KEY_PASSWORD=your_key_password
```

Build the APK:

```bash
./gradlew :TMessagesProj_AppStandalone:assembleAfatStandalone
```

The APK will be available in:

```text
TMessagesProj_AppStandalone/build/outputs/apk/afat/standalone/
```

## Credits

VEDAgram is based on [Finegram](https://github.com/Th3Nekit/Finegram) by [Th3Nekit](https://github.com/Th3Nekit), which is based on [Cherrygram](https://github.com/arsLan4k1390/Cherrygram) and [Telegram for Android](https://github.com/DrKLO/Telegram).

Please retain the original licenses and notices:

- [LICENSE](LICENSE)
- [LICENSE.PluginManager](LICENSE.PluginManager)
- [LICENSE.telegram-gpl2](LICENSE.telegram-gpl2)
- [NOTICE](NOTICE)
