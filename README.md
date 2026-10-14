# Username Picker

![demo](/preview/demo.gif)

A small single-page app that picks random usernames for me. Names are sorted into categories, and each one comes with its meaning.

## Categories

- **Slavic**: Russian and Ukrainian words (Zarnitsa, Metel, Iskra)
- **Japanese**: Japanese-inflected words (Kagerou, Shigure, Hotaru)
- **Norse**: Old Norse and Nordic words (Myrkr, Hrafn, Skuggi)
- **Latin**: Latin roots (Umbra, Vesper, Tenebrae)
- **Invented**: Made-up names chosen for their sound (Kyrenth, Ashveil, Nyxari)

## Features

- Roll a random name from all categories or from one
- See the meaning and category of each name
- Save favorites (stored in your browser, so they stay on your device)
- Copy a name with one click
- Browse every name, grouped by category
- Light and dark mode follow your system setting
- Press Space to roll


## Adding names

Names live in the `DATA` object near the bottom of `username-picker.html`. Each entry is `["Name", "meaning"]`. Leave the meaning empty (`""`) for names with no set meaning.

```js
"Norse": { c: "#0369a1", n: [
  ["Hrafn", "raven"],
  ["YourNewName", "its meaning"]
]}
```

To add a category, add a new key with its own color (`c`) and list of names (`n`). The chips and the browse list update automatically.

## Tech

Plain HTML, CSS and JavaScript in one file. No frameworks or dependencies. Fonts load from Google Fonts and fall back to system fonts if offline.