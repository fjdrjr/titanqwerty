# TitanQwerty

This Fork of [FinQwerty app by anssih](https://github.com/anssih/finqwerty) was created to add support for the Unihertz Titan Pocket (German so far)

Various keyboard layouts for the physical QWERTY keyboards of the following Android phones:

- Unihertz Titan Pocket (German so far)
- BlackBerry KEYone **Android 7.1 only** (Danish, Finnish, German, Norwegian, Swedish)
- BlackBerry Priv (Danish, Finnish, German, Norwegian, Swedish)
- F(x)tec Pro1 (Bulgarian, Czech, Danish, Finnish, German, Greek, Hungarian, Italian, Norwegian, Polish, Portuguese, Slovakian, Swedish, Swiss French, Ukrainian, U.S., U.S. international)
- Gemini PDA (Bulgarian, Finnish, Swedish)
- Livermorium Keyboard Moto Mod (Danish, Finnish, German, Norwegian, Swedish)
- Motorola Droid 4 (Finnish, Swedish)
- Motorola Photon Q 4G (Finnish, Swedish)
- Samsung Galaxy S Relay 4G (Finnish, Swedish)

See the [FinQwerty website](https://android.onse.fi/finqwerty/) for detailed layout maps. - does not apply for Unihertz Titan Pocket - see below -

The layouts are provided via the Android standard layouts mechanism and are selectable in Android settings - no root required.
An in-app workaround is also included for BlackBerry phones that do not have those settings.

## Installing

1. Download the forked .apk with Unihertz Titan Pocket support from the [release](https://github.com/fjdrjr/finqwerty/releases) section
2. On your Titan pocket, tap the .apk file to install it
   NOTE: Unknown sources must be enabled to install the App from file.
2. Accept eventual security warnings

## Enabling

1. Open app and tap on "physical keyboard settings"
2. Tap on "aw9523-key" - that is the name of Titan Pocket's physical keyboard device
3. Tap on "Add layouts" underneath the offered selection
4. Scroll down the list until you find "FinQwerty Unihertz Titan Pocket"
5. Enable the switch behind the desired layout
6. Go back and choose the layout you just enabled in the step before as your active keyboard layout

## Titan Pocket specific

NOTE 1: This layout files are designed for use with virtual keyboard turned of since the additional characters are mapped to SYM+letter

NOTE 2: For some capital letters or symbols SYM+Shift+letter must be pressed

NOTE 3: There is currently no keylayout chart so you simply have to try all letters with SYM-key to find the positions of symbols


## Building

Python 3 is required to build FinQwerty.

The project uses Gradle and can be built with Android Studio or via commandline, for example:

```
export JAVA_HOME="$HOME/android-studio/jre"
export ANDROID_HOME="$HOME/Android/Sdk"
./gradlew assembleDebug
```

## Layout files

Some of the Pro1 layouts (fin/nor/swe and cze qwerty) are generated from other layouts automatically by `generate_layouts.py`
during the build process and are therefore not found in this repository.

For convenience, all the `.kcm` files, including automatically generated ones, from the latest FinQwerty release can be found here:
https://android.onse.fi/finqwerty/kcm/

## License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.

