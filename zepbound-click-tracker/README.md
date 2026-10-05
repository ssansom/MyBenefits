# Pen Click Tracker

A single-file, offline web page for tracking click-counted partial doses from a
multi-dose Zepbound KwikPen (e.g. taking 2.5 mg, 3.75 mg … from a 15 mg pen).

Open `index.html` in a browser (or host it anywhere static, e.g. GitHub Pages).
Data is stored in the browser's `localStorage`; use **Export backup** to save a copy.

## What it does

- Shows how many clicks to dial for each dose step (2.5 – 7.5 mg in 1.25 mg steps).
- Logs doses per pen with date and notes; shows the next weekly due date.
- For every dose step, shows how many doses are left in the current pen (or a
  fresh pen) and how much would be left over / discarded, noting when the
  leftover still covers a smaller dose.
- Keeps history of previous pens.

## Assumptions (editable under *Pen settings*)

| Setting | Default |
| --- | --- |
| Clicks per full labeled dose | 60 |
| Full doses per pen | 4 (240 clicks) |
| Extra/overfill clicks | 0 |
| Priming clicks per injection | 0 |

With a 15 mg pen this is 0.25 mg per click: 2.5 mg = 10, 3.75 mg = 15, 5 mg = 20,
6.25 mg = 25, 7.5 mg = 30 clicks.

Click counting is not in the manufacturer's instructions; confirm your plan with
your prescriber or pharmacist.
