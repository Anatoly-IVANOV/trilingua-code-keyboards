**Trilingua Code Keyboards**

A solution for the creative multilingual pro tired of switching between languages and special characters’ palettes…

# Description

*Trilingua Code Keyboards* layouts improve the work of those who touch-type in English, French and Russian — like myself — plus write code daily, while insisting on typographic niceties and the preservation of industry-standard `J K L` shortcuts of audio/video editing software timeline control built for QWERTY.

> [!TIP]
> No language switching via `⌃ ⌥ space` required — if you stay bilingual.

I’ve created 2 keyboard layouts:

1. **EN+FR Trilingua Code**: combines the English QWERTY standards with French accented letters, specially optimized for coding. It includes an inverted number row for easy access to frequently used coding symbols and with a `Shift` and `Alt` integrates the French diacritics almost like on an AZERTY keyboard.

2. **RU Trilingua Code**: this layout mirrors the structure of *EN+FR Trilingua Code*, facilitating a fluid transition for those proficient in Russian as well. It still requires some work for a complete replica.

> [!NOTE]
> Those are for MacOS, but you can find inspiration for your OS of choice.

# Details of the layouts

**No modifiers**
<img src="keyboard_layouts_images/TrilinguaCode_EN+FR_modifiers_none_20231230.png" width="100%">

**Shift modifier**
<img src="keyboard_layouts_images/TrilinguaCode_EN+FR_modifiers_shift_20231230.png" width="100%">

**Alt modifier**
<img src="keyboard_layouts_images/TrilinguaCode_EN+FR_modifiers_alt_20231230.png" width="100%">

**Alt Shift modifier**
<img src="keyboard_layouts_images/TrilinguaCode_EN+FR_modifiers_shift+alt_20231230.png" width="100%">

# Project Goals

- **Multilingual Coding Efficiency**: Aimed at bridging the gap between English, French, and Russian in coding environments, these layouts simplify the language switching process for touch-typing programmer-designer-filmmakers who want to preserve the access to familiar shortcuts.
- **User-Centric Design**: The layouts are crafted to be intuitive for both bilingual and trilingual users, minimizing the learning curve and maximizing typing proficiency.
- **Compatible with built-in MacBooks’ keyboards**: Yes, the latest split ergo marvels layered with [ZMK](https://github.com/zmkfirmware/zmk) are superb, but not always available.

# Installation

## MacOS

- download the keyboard bundles from the `Releases`
- unzip into your `~/Library/Keyboard Layouts/` user Library or `/Library/Keyboard Layouts` if you want all users to have access to the keyboards
- go to `System Preferences > Keyboard > Input Sources` or some harder-to-find-with-each-MacOS-release location to enable the keyboards
- most probably, you will have to log-out… gone are the easy days of MacOS 10.0
- I then tend to disable the built-in stock English and French layouts

## All other OSes

- for now, I haven’t compiled anything for Windows or Linux
- you can build your own variants based off the images

# Special features

- top rows optimized for direct access to various brackets **( )**, **[ ]** and **$** dollar sign used in programming
- **“” «»**  typographer’s quotes for English and French in one place
- **—**  m-dash
- **–**  n-dash
- **…**  typographical ellipsis
- **→**  arrow frequently used in design and documentation
- **°**  degree symbol (yes, I do a lot of CAD [@idelekka](https://idelekka.com) as well)
- **≈**  approximate equality sign
- **ø**  diameter symbol
- **€**  Euro, **£** Pound currency symbols

# Uninstall default keyboards

## MacOS

MacOS insists on keeping at least 1 Latin keyboard they ship. So when you cycle through the layouts — I’m using `⌘ Space` — you’ll get English twice.

To remove the no longer needed layouts:

1. Change the current input source to the *Trilingua Code* custom keyboard layout.

2. Open `~/Library/Preferences/com.apple.HIToolbox.plist` (if needed, convert the binary `.plist` to `XML` with `plutil -convert xml1`).

3. Remove the input source or input sources you want to disable from the `AppleEnabledInputSources` dictionary.

4. If there is an `AppleDefaultAsciiInputSource` key, remove it.

5. Save the new version of `~/Library/Preferences/com.apple.HIToolbox.plist`.

6. Restart.

   > [!IMPORTANT]
   > Logging out and back in is not enough.

# Modification

Feel GPL-free to modify to suit your language (my German is decaying, hence the lack of its support, but you get the umlaut idea).

# Feedback and suggestions

I’m continuously improving and evolving the keyboard layouts and welcome any feedback and contributions.

# To-do

- complete the mirror of the EN+FR to RU
- remove several redundancies — I was testing different placements
