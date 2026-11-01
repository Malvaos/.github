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
    <td width="50%"><img alt="Malva OS, light: menu bar, Control Center, dock" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/hero-light.jpg"></td>
    <td width="50%"><img alt="Malva OS, dark: menu bar, Control Center, dock" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/hero-dark.jpg"></td>
  </tr>
</table>

## Why Malva

Linux has the engine. What it often lacks is a desktop that feels like one person designed all of it. Malva OS is that attempt: one design language, one set of tokens, and a shell, apps and toolkit that all read from it - so changing a token restyles everything at once, and nothing looks like it came from somewhere else.

The mark is a mallow flower: five heart-shaped petals around a leaf-green centre. Each petal has one small notch at the tip. The notch is our bite, the same small cut every time.

## How it is designed

- **Black and white, with the logo's colour.** Surfaces, text and borders are neutral. One colour is strong, the logo's plum (a lighter orchid in dark), and it appears only where something can be acted on or is selected: primary buttons, switches that are on, selection, focus, links.
- **One token file.** Every colour, radius, space, type size and timing lives in a single JSON file that generates the Slint, C++, Rust, CSS and SVG sides, so they cannot drift apart.
- **Quiet motion.** 90 ms for a press, 160 ms for hover, 240 ms for things that open, with a small spring only where something arrives. Motion explains; it never decorates.
- **Every state exists.** Default, hover, pressed, focus and disabled - for every control, in both themes, with a focus ring that shows for the keyboard only.
- **Safe by default.** Destructive actions are red and never the default button. Colour is never the only signal: it always comes with text or an icon.

### Palette

| Role | Light | Dark |
|---|---|---|
| Background | ![](https://img.shields.io/badge/-%23F5F5F7-F5F5F7?style=flat-square) `#F5F5F7` | ![](https://img.shields.io/badge/-%23161617-161617?style=flat-square) `#161617` |
| Surface | ![](https://img.shields.io/badge/-%23FFFFFF-FFFFFF?style=flat-square) `#FFFFFF` | ![](https://img.shields.io/badge/-%231E1E1F-1E1E1F?style=flat-square) `#1E1E1F` |
| Text | ![](https://img.shields.io/badge/-%231D1D1F-1D1D1F?style=flat-square) `#1D1D1F` | ![](https://img.shields.io/badge/-%23F5F5F7-F5F5F7?style=flat-square) `#F5F5F7` |
| Secondary text | ![](https://img.shields.io/badge/-%2386868B-86868B?style=flat-square) `#86868B` | ![](https://img.shields.io/badge/-%238E8E93-8E8E93?style=flat-square) `#8E8E93` |
| Border | ![](https://img.shields.io/badge/-%23E5E5EA-E5E5EA?style=flat-square) `#E5E5EA` | ![](https://img.shields.io/badge/-%232C2C2E-2C2C2E?style=flat-square) `#2C2C2E` |
| Accent | ![](https://img.shields.io/badge/-%238C3274-8C3274?style=flat-square) `#8C3274` | ![](https://img.shields.io/badge/-%23DC73C2-DC73C2?style=flat-square) `#DC73C2` |
| Danger | ![](https://img.shields.io/badge/-%23D6414F-D6414F?style=flat-square) `#D6414F` | ![](https://img.shields.io/badge/-%23FF7A85-FF7A85?style=flat-square) `#FF7A85` |
| Success | ![](https://img.shields.io/badge/-%233F8A1E-3F8A1E?style=flat-square) `#3F8A1E` | ![](https://img.shields.io/badge/-%237FD35A-7FD35A?style=flat-square) `#7FD35A` |

## What we are building

| Layer | What it is |
|---|---|
| **Malva UI** | The design system as code: a Slint component library (69 parts, dark and light) with C++, Rust, iced, CSS and SVG generated from the same tokens, 130 symbols and 20 app icons. |
| **Shell** | Menu bar with Wi-Fi, Bluetooth, battery, sound, calendar, Control Center, notifications, on-screen display and power; a dock with magnification. |
| **Apps** | The Files app front end is built on the kit. Settings, task manager, backup, disk manager, terminal, media, notes, calculator, image viewer, browser, installer and login screen are designed as interactive prototypes. |
| **Wallpapers** | A light and a dark one: silver and graphite, with a soft bloom of the logo's colour. |

<table>
  <tr>
    <td width="33%"><img alt="Files, dark" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/shot-files.jpg"></td>
    <td width="33%"><img alt="Dock with its context menu, light" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/shot-dock.jpg"></td>
    <td width="33%"><img alt="Notification centre, dark" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/shot-notifications.jpg"></td>
  </tr>
  <tr align="center">
    <td>Files</td><td>Dock</td><td>Notification centre</td>
  </tr>
</table>

### Malva UI in one look

```slint
import { Theme, Button, ButtonKind, TextField, Card } from "@malva/malva.slint";

export component Example inherits Window {
    default-font-family: "Inter";
    background: Theme.bg;
    // Theme.dark = true;  flips every colour of every component
    Card {
        VerticalLayout {
            padding: 24px;
            spacing: 12px;
            TextField { placeholder: "Device name"; }
            Button { text: "Save"; kind: ButtonKind.primary; }
        }
    }
}
```

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/components-dark.jpg">
  <img alt="Every part of the Malva UI kit on one board" src="https://raw.githubusercontent.com/Malvaos/.github/main/profile/assets/components-light.jpg">
</picture>

## Status

Early. Today this is the design system, the UI toolkit, the shell and Files app front ends built on it, and interactive prototypes of the other apps. Watch the repositories below for releases.

- [Malva-ui-toolkit](https://github.com/Malvaos/Malva-ui-toolkit) - the UI toolkit
- [malva-design](https://github.com/Malvaos/malva-design) - brand, tokens, guidelines and the app prototypes

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
