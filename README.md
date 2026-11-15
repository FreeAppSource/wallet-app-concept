# Wallet App Concept

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Fekry Studio** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `wallet-app-concept-fekry-studio.sketch` by **Fekry Studio**: one route per artboard, with the artboard's layout, colours, images and text.

![Wallet App Concept screens](./showcase.jpg)

## 📱 Screens (15 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **Splash** · start screen | `src/app/splash.jsx` | 375 × 812 | 1 |
| 2 | **home** | `src/app/home.jsx` | 375 × 812 | 3 |
| 3 | **merchent page** | `src/app/merchent-page.jsx` | 375 × 954 | 2 |
| 4 | **points** | `src/app/points.jsx` | 375 × 812 | 2 |
| 5 | **merchents** | `src/app/merchents.jsx` | 375 × 812 | 2 |
| 6 | **profile** | `src/app/profile.jsx` | 375 × 812 | 5 |
| 7 | **merchents - search** | `src/app/merchents-search.jsx` | 375 × 812 | 3 |
| 8 | **Settings** | `src/app/settings.jsx` | 375 × 812 | 2 |
| 9 | **wallet** | `src/app/wallet.jsx` | 375 × 812 | 2 |
| 10 | **offer details** | `src/app/offer-details.jsx` | 375 × 812 | 2 |
| 11 | **suggMerchents** | `src/app/suggmerchents.jsx` | 375 × 812 | 2 |
| 12 | **pay** | `src/app/pay.jsx` | 375 × 812 | 4 |
| 13 | **pay - fail** | `src/app/pay-fail.jsx` | 375 × 812 | 5 |
| 14 | **pay - sucsess** | `src/app/pay-sucsess.jsx` | 375 × 812 | 5 |
| 15 | **pay w-merchent ID** | `src/app/pay-w-merchent-id.jsx` | 375 × 812 | 4 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (DM Sans, Inter), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/wallet-app-concept> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Wallet App Concept** design by **Fekry Studio**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Fekry Studio](https://www.sketchappsources.com/contributor/fekrystudio) |
| Original design | [Wallet App Concept](https://dribbble.com/shots/7006278-hokum-Free-Sketch-Template-for-a-Wallet-app) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4094-wallet-app-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/FekryStudio> |
| Twitter | <https://twitter.com/Mohamedfekryyy> |
| Original file | `wallet-app-concept-fekry-studio.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Wallet App Concept" by Fekry Studio (https://dribbble.com/shots/7006278-hokum-Free-Sketch-Template-for-a-Wallet-app), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4094-wallet-app-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
