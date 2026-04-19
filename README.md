# 📐 Area Calc — Multi-Section Rectangular Area Calculator

A lightweight, zero-dependency single-file web app for calculating the area of multiple rectangular sections and tracking their combined total — built for field measurements, land surveys, and construction layouts.

> **No install. No build step. No internet required after first load.** Just open the `.html` file in any browser.

---

## ✨ Features

- **Multi-unit input** — enter dimensions in metres, feet, cm, mm, inches, yards, or kilometres
- **Add multiple rectangles** — each section is calculated and listed individually
- **Running total** — the combined area updates automatically with every addition
- **12 output units** — results shown simultaneously in all units
- **Delete individual entries** — with a 4-second undo window
- **Clear all** — reset the entire session in one click
- **Keyboard friendly** — press `Enter` to add a rectangle without touching the mouse
- **Input validation** — catches empty or invalid values with a clear error message
- **Responsive** — works on desktop and mobile browsers

---

## 📦 Output Units

Results are displayed in all of the following units simultaneously:

| Unit | Description |
|------|-------------|
| m² | Square metres |
| sq feet | Square feet |
| mm² | Square millimetres |
| cm² | Square centimetres |
| Acre | International acre |
| Cent | Used widely in South India (1 acre = 100 cent) |
| Gunta / Guntha | Common in Karnataka, Maharashtra, AP, Telangana |
| Marla | Used in North India, Punjab, Haryana |
| Ground | Used in Tamil Nadu (1 ground ≈ 222.97 m²) |
| sq yards | Square yards |
| Hectare | Metric land area unit |
| km² | Square kilometres |

---

## 🚀 Usage

1. **Download** `area-calculator.html`
2. **Open** it in any modern browser (Chrome, Firefox, Safari, Edge)
3. **Select** your input unit from the dropdown
4. **Enter** the Length (L) and Breadth (B) of a rectangular section
5. **Click ＋** (or press `Enter`) to add it
6. Switch between **Last Added** and **Total Area** tabs to view results
7. **Repeat** for each additional section

---

## 🖼️ Interface Overview

```
┌─────────────────────────────────┐
│  INPUT UNIT: [Metre (m)     ▾]  │
│                                 │
│  L — Length    B — Breadth      │
│  [ 12.5     ]  [ 8.0      ] [＋]│
└─────────────────────────────────┘

┌─────────────────────────────────┐
│  RECTANGLES ADDED      Clear All│
│  1   12.5 × 8.0 m    100 m²  ✕ │
│  2   6.0  × 4.5 m     27 m²  ✕ │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│  AREA RESULTS         2 sections│
│  [ Last Added ] [ Total Area ]  │
│                                 │
│  m²         sq feet             │
│  127         1367.01            │
│  mm²         cm²                │
│  127000000   1270000            │
│  ...                            │
└─────────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Layer | Choice |
|-------|--------|
| Structure | HTML5 |
| Styling | CSS3 (variables, grid, animations) |
| Logic | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts — Sora + Space Mono |
| Dependencies | **None** |

Everything lives in a **single `.html` file** — no frameworks, no bundlers, no server needed.

---

## 📐 Conversion Reference

All conversions are based on the input being converted to **m²** internally, then scaled to each output unit:

| Input Unit | Factor to m² |
|------------|-------------|
| Metre | 1 |
| Foot | 0.092903 |
| Centimetre | 0.0001 |
| Millimetre | 0.000001 |
| Inch | 0.00064516 |
| Yard | 0.836127 |
| Kilometre | 1,000,000 |

---

## 💡 Use Cases

- 🌾 **Agriculture** — measure multiple farm plots, add them up for total field area
- 🏗️ **Construction** — calculate room-by-room floor area for a building
- 🏡 **Real estate** — convert land dimensions to local units (Cent, Gunta, Ground, Marla)
- 📏 **Site surveys** — quickly total irregularly shaped land split into rectangular sections
- 🎓 **Education** — demonstrate area calculation and unit conversion concepts

---

## ⚠️ Limitations

- **Rectangular sections only** — irregular polygons, circles, or triangles are not supported
- **No data persistence** — entries are cleared when the page is refreshed (session-only)
- **Internet for fonts** — Google Fonts are loaded from CDN; the app works offline but will fall back to system fonts

---

## 🤝 Contributing

Contributions are welcome! Some ideas for future improvements:

- [ ] Export results as PDF or CSV
- [ ] Name/label individual rectangles
- [ ] Support triangular and circular sections
- [ ] LocalStorage persistence across sessions
- [ ] Shareable URL with encoded entries

To contribute: fork the repo, make your changes to `area-calculator.html`, and open a pull request.

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

<p align="center">Made for farmers, builders, and surveyors who just want the numbers. 🌱</p>
