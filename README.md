# Notes about Nokia 6300 4G development

- os version: `kaios v2.5.4+` (`build 12.00.17.01`)

## Install ADB on the computer

From MacOS, install `brew` if necessary:

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Then install the android platform tools:

```bash
brew install --cask android-platform-tools
```

## Enable ADB and/or DevTools on the phone
- Visit menu.kaios.dev on your KaiOS device
- Settings app will open with options to enable debugging: Debugger -> ADB and DevTools

## Ensure phone is accessible by ADB

- Connect the phone with a USB cable
- Run command `adb devices`from your computer
- A device should appear, ex: 
```bash
imac:~ user$ adb devices
List of devices attached
a1d8bf2	device
```

## References

- https://www.kaiostech.com/learn-to-develop-for-the-kaios-operating-system-with-these-resources/
- https://developer.kaiostech.com/docs/
- https://community.phones.nokia.com/discussion/4840/i-want-to-enter-developer-mode
