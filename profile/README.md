<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/malva-logo-horizontal-reverse.svg">
  <img alt="Malva OS" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/malva-logo-horizontal.svg" width="340">
</picture>

### A Linux desktop designed to beat macOS at design and stability.

Calm by default. Consistent everywhere. Every state designed.

</div>

<br>

<table>
  <tr>
    <td width="50%"><img alt="Malva OS desktop, dark: menu bar, control center, dock" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/desktop-dark.jpg"></td>
    <td width="50%"><img alt="Malva OS desktop, light" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/desktop-light.jpg"></td>
  </tr>
</table>

## Why Malva

Linux has the engine. What it often lacks is a desktop that feels like one person designed all of it. Malva OS is that attempt: one design language, one set of tokens, and a shell, apps and toolkit that all read from it - so changing a setting restyles everything at once, and nothing looks like it came from somewhere else.

The mark is a mallow flower: five heart-shaped petals around a leaf-green centre. Each petal has one small notch at the tip. The notch is our bite, the same small cut every time.

## How it is designed

- **One dial.** *Balance* runs from Soft to Crisp. Radii, type weight, shadows and contrast move together, so the look stays coherent at every setting. The default is the tuned middle.
- **Dusty orchid in dark, plum in light.** Surfaces tint toward plum, never grey. The accent is capped so it is never neon.
- **Quiet motion.** 120 ms for feedback, 240 ms for overlays, a small spring only where something arrives. *Reduce motion* sets every duration to zero.
- **Every state exists.** Default, hover, pressed, focus and disabled - for every control, in both themes, with keyboard focus rings that read on any background.
- **Safe by default.** Destructive actions are rose and never the default button. Fields validate after you leave them, not while you type. Colour is never the only signal. Touch targets are 44 px.

### Palette

| Role | Dark | Light |
|---|---|---|
| Background | ![](https://img.shields.io/badge/-%231D101C-1D101C?style=flat-square) `#1D101C` | ![](https://img.shields.io/badge/-%23F6F0F6-F6F0F6?style=flat-square) `#F6F0F6` |
| Surface | ![](https://img.shields.io/badge/-%232A1929-2A1929?style=flat-square) `#2A1929` | ![](https://img.shields.io/badge/-%23FBF8FB-FBF8FB?style=flat-square) `#FBF8FB` |
| Accent | ![](https://img.shields.io/badge/-%23D47ABC-D47ABC?style=flat-square) `#D47ABC` | ![](https://img.shields.io/badge/-%237E376A-7E376A?style=flat-square) `#7E376A` |
| Danger | ![](https://img.shields.io/badge/-%23FF8A94-FF8A94?style=flat-square) `#FF8A94` | ![](https://img.shields.io/badge/-%23C0414E-C0414E?style=flat-square) `#C0414E` |
| Success | ![](https://img.shields.io/badge/-%237BC74D-7BC74D?style=flat-square) `#7BC74D` | ![](https://img.shields.io/badge/-%233F7F1B-3F7F1B?style=flat-square) `#3F7F1B` |

## What we are building

| Layer | What it is |
|---|---|
| **Malva UI** | The design system as a Slint toolkit: one `Theme`, 58 components, 87 icons, dark and light, accessibility switches. |
| **Shell** | Menu bar with Wi-Fi, Bluetooth, battery, sound, calendar, control center, notifications, on-screen display and power; a dock with cosine magnification. |
| **Apps** | Files, Settings, task manager, backup, disk manager, terminal, media, notes, calculator, image viewer, browser, installer and login screen. |
| **Wallpapers** | *Dusk* and *Dawn*, the two moods of the system. |

<table>
  <tr>
    <td width="33%"><img alt="Files" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/app-files.jpg"></td>
    <td width="33%"><img alt="Task manager" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/app-ltask.jpg"></td>
    <td width="33%"><img alt="Settings" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/app-settings.jpg"></td>
  </tr>
  <tr align="center">
    <td>Files</td><td>Task manager</td><td>Settings</td>
  </tr>
</table>

### Malva UI in one look

```slint
import { Theme, Button, TextField, Card } from "@malva";

export component Example inherits Window {
    background: Theme.bg;
    Card {
        TextField { placeholder: "Device name"; }
        Button { text: "Save"; }
    }
}
// Theme.dark = false;  Theme.balance = 70;  Theme.reduce-motion = true;
```

<img alt="Malva UI gallery: data widgets" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/malva-ui-widgets.jpg">

## Status

Early. Today this is the design system, the UI toolkit, the shell design and interactive app prototypes. Watch the repositories below for releases.

<!-- Add repository links here as they go public, for example:
- [malva-slint](https://github.com/Malvaos/malva-slint) - the UI toolkit
-->

## Get involved

- **Ideas and feedback:** open an issue or start a discussion in any repository.
- **Design:** the rules above are the contract. If a screen breaks one, that is a bug worth reporting.
- **Code:** read the repository's README first; keep changes small and say which state or theme you tested.

<div align="center">
<br>
<img alt="" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/malva-mark.svg" width="44">
<br>
<sub>Malva OS - five petals, one notch.</sub>
</div>
