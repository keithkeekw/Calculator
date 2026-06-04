> [!NOTE]
> This is my first code vibing project. 😄

# 🧮 Web Calculator

A clean, responsive calculator built with **React** and **Tailwind CSS** — all from CDNs, so there's **no build step**. Just open one HTML file in your browser.

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-CDN-38BDF8?logo=tailwindcss&logoColor=white)
![No Build](https://img.shields.io/badge/build-none-2FA084)
![License](https://img.shields.io/badge/license-MIT-1F6F5F)

---

## ✨ Features

- **Basic arithmetic** — add, subtract, multiply, divide, percent, sign toggle (±), decimals
- **History tape** — every calculation is logged; click any entry to reload its result, or clear the whole list
- **Dark / light theme** — toggle with one click, remembered across reloads (`localStorage`), with no flash on load
- **Full keyboard support** — type your way through every operation
- **Responsive layout** — calculator and history sit side-by-side on desktop and stack on mobile
- **Safe math** — no `eval()`; arithmetic uses an explicit switch with divide-by-zero handling and float-noise cleanup
- **Custom green color palette** — see below

---

## 📸 Demo

> _Add a screenshot or GIF here, e.g._ `![Calculator screenshot](./screenshot.png)`

---

## 🚀 Getting Started

No installation, no dependencies to download, no build tooling.

```bash
# Clone the repository
git clone https://github.com/<your-username>/calculator.git
cd calculator
```

Then open the file in your browser:

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

> ℹ️ An internet connection is required on first load, since React, Tailwind CSS, and Babel are loaded from CDNs.

---

## ⌨️ Keyboard Shortcuts

| Key            | Action            |
| -------------- | ----------------- |
| `0`–`9`        | Enter digits      |
| `.`            | Decimal point     |
| `+` `-` `*` `/`| Operators         |
| `Enter` or `=` | Equals            |
| `%`            | Percent           |
| `Backspace`    | Delete last digit |
| `Escape`       | Clear all (AC)    |

---

## 🛠️ Tech Stack

- **React 18** — UI and state (loaded via UMD CDN)
- **Tailwind CSS** — styling (CDN, with inline config for `darkMode: 'class'` and custom colors)
- **Babel standalone** — transpiles JSX in the browser, keeping the project build-free

---

## 🎨 Color Palette

| Color     | Hex       | Usage                                                        |
| --------- | --------- | ----------------------------------------------------------- |
| Neutral   | `#EEEEEE` | Light-mode background, display & number surfaces, light text |
| Light green | `#6FCF97` | Operator buttons, accents, hover highlights               |
| Mid green | `#2FA084` | Equals button, active operator state                        |
| Dark green | `#1F6F5F` | Dark-mode background/card, history header, pressed states  |

---

## 📁 Project Structure

```
calculator/
└── index.html   # The entire app — markup, styling config, and React component
```

Everything lives in a single self-contained file.

---

## 📝 Notes & Limitations

- **Immediate-execution chaining** — operations evaluate left-to-right like a standard pocket calculator (`2 + 3 × 4` = `20`), not by operator precedence (`14`).
- **CDN dependency** — first load needs internet access. For offline use or production performance, the natural next step is migrating to a [Vite](https://vitejs.dev/) + Tailwind build.

---

## 📄 License

[MIT](./LICENSE) — feel free to use, modify, and share.
