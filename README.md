# Customary vs Metric Units

Students pour liquids, balance everyday objects and convert between systems, to see how customary and metric units compare.

**Live site:** <https://jontaylormed.github.io/customary-metric-units/>

**Source:** <https://github.com/jontaylormed/customary-metric-units>

**Site created by Claude and Jon Taylor.**

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---

## What it does

| Section | What the student does |
|---|---|
| Quick Reference Guide | Reads how units relate within each system, plus the key conversions between systems |
| Liquid Pouring Lab | Picks a customary unit, turns on the faucet, and watches the same amount fill customary and metric containers side by side |
| Real-World Volume Comparisons | Compares everyday amounts, from a soda can to an Olympic pool, in both systems |
| Mass Balance Lab | Puts everyday objects on a two-pan scale, watches it tip, and switches the readout between customary and metric |
| Challenge Questions | Works out how many of one object balance another, then tests it on the scale |
| Unit Converter | Converts length, capacity, weight and mass, and temperature, in both directions |
| Quiz | Answers 10 multiple-choice questions in a random order |

## Who it's for

Grades 4–7.

Common Core State Standards for Mathematics:

| Standard | What it asks |
|---|---|
| 4.MD.A.1 | Know the relative sizes of units within one system (km, m, cm; kg, g; lb, oz; l, ml) |
| 5.MD.A.1 | Convert among different-sized units within one measurement system |
| 6.RP.A.3d | Use ratio reasoning to convert measurement units |

## How it teaches

- **See it first.** Students pour and weigh before they convert. The labs show how big a cup or a kilogram is before the converter gives a number.
- **Side by side, the same way every time.** Customary is orange and metric is blue throughout. Every label also names its system and unit, so color is never the only cue.
- **Check every claim.** A rounded value is marked "≈" and rounds correctly to the digits shown. An exact value, like 1 in = 2.54 cm, is marked exact.

## How the math was checked

- **Checks page:** [`checks.html`](https://jontaylormed.github.io/customary-metric-units/checks.html) runs 215 checks in the browser. It compares every number on the page with exact definitions: 1 in = 2.54 cm, 1 lb = 453.59237 g, and 1 US gallon = 231 cubic inches. All 215 pass. The checks cover:
  - every row of the reference guide;
  - the Liquid Lab's unit sizes and container capacities;
  - the volume comparisons and the masses of the objects;
  - each challenge answer, worked from the numbers in its own hint;
  - every quiz answer key;
  - the converter at sample values, including the temperature anchors −40°, 0°, 32°, 37°, 98.6°, 100° and 212°;
  - the keyboard flow slider, button names, color contrast and the reduced-motion rule;
  - a scan of the page for network requests and storage.
- **Fixed after checking:** an earlier version showed rounded sizes as exact, and four customary challenge answers didn't follow from their own rounded numbers. Its containers were also off by up to 3 mL, and the boiling-point question didn't say "at sea level." All are fixed.
- **Known limits:** object masses are typical values, such as a medium apple or a newborn baby, not exact ones. Challenge answers that use rounded numbers say so.

## Accessibility

- **Keyboard:** everything works with the keyboard, and focus outlines are visible.
  - The section tabs, lab buttons, converter boxes and quiz choices are standard buttons and fields.
  - The Liquid Lab's flow control is a slider: arrow keys move it 5%, Page Up and Page Down 25%, and Home and End go to 0% and 100%.
  - Each scale button names its object, such as "Add Apple to the left pan."
- **Contrast:** text meets the WCAG 2.1 AA target of 4.5:1. Examples:
  - body text, 13.6:1;
  - white on the orange buttons, 5.2:1, and on the blue buttons, 5.8:1;
  - grey labels, 5.4:1 or better;
  - the quiz's "Correct" text, 4.9:1.
- **Screen readers:** converter answers, quiz feedback, revealed challenge answers and the balance result are read aloud when they change. The customary/metric switch says whether it is on.
- **Motion:** when the device asks for reduced motion, the dripping faucet, the pulsing overflow badge and the tipping scale stop animating.
- **Text size:** there is no separate setting; the page follows browser zoom.

## Privacy

No accounts, no tracking, no cookies and no stored data. The page makes no network requests: its two typefaces are built into the file, and `checks.html` confirms nothing loads from outside.

## Running it

Open `index.html` in any modern browser.

`checks.html` reads the tool, so open it from the live site or any local web server, not as a file.

**Publishing:** GitHub Pages, deployed from the `main` branch at the repository root. There is no build step.

## License

[CC BY-NC-SA 4.0](LICENSE). Free to share and adapt for non-commercial use, with credit, under the same license.

The bundled typefaces have their own license, and their license files are in [`fonts/`](fonts/):

| Typeface | Used for | Designer | License |
|---|---|---|---|
| Fredoka One | Headings | Milena Brandão | [SIL Open Font License 1.1](fonts/OFL-fredokaone.txt) |
| Nunito | Body text | The Nunito Project Authors | [SIL Open Font License 1.1](fonts/OFL-nunito.txt) |
