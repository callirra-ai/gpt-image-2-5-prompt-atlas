# Fintech Dashboard

![A fintech operations dashboard with four KPI tiles, two charts and a five-row transaction table](preview.jpg)

A fintech operations dashboard with real, internally consistent data: four KPI tiles whose deltas agree with their own sparklines, two charts whose legends match the series actually drawn, and a transaction table whose five amounts sum exactly to the total printed in its footer. Use it for product marketing, pitch decks, UI case studies and any mock where fake data has to survive being read.

**This is the heaviest text prompt in the atlas** — around sixty exact strings plus one arithmetic requirement — and it passed on the first render.

## Try the prompt

```text
A fintech operations dashboard, 16:9, screen only — a flat rectangular interface shown straight on with no
device, no desk, no hand and no perspective. This is a UI mock with real committed data, not a photograph.

LAYOUT — fixed regions, no overlap
- Top bar, 9% of the frame height: product name at the left, the date-range control and one account chip at the
  right, and a single hairline rule closing the bar across the full width.
- Left rail, 15% of the frame width: six navigation items stacked with even spacing. The first is active, marked
  by a 3 px accent bar on its left edge and a tinted row background.
- Main area, to the right of the rail, split into three stacked panels with even gaps: KPI row 24% of the main
  height, charts row 36%, table panel 40%.
- KPI row: four equal tiles side by side, each with its label above its value, its value above its delta, and
  one small sparkline at the tile's right edge.
- Charts row: a line chart at 62% of the row width and a stacked bar chart at 38%, with one gutter between them.
- Table panel: a six-column table with a header row, five data rows and a footer line.
- Every panel sits on a flat ground with a 1 px border. No drop shadows anywhere.

DATA — this must be internally consistent, and the arithmetic must close
- Net volume: $4.82M, up 12.4%, sparkline rising left to right.
- Active accounts: 18,204, up 3.1%, sparkline rising left to right.
- Auth rate: 97.6%, down 0.4%, sparkline falling left to right.
- Settlement time: 1.9 days, down 0.3 days, sparkline falling left to right.
  Each delta's sign must agree with the direction its own sparkline moves. All four sparklines appear.
- The line chart has exactly two series, each with a legend entry, and no legend entry without a series.
- The five table amounts below sum to exactly $50,671.50, which is the figure stated in the table footer.

EXACT VISIBLE TEXT — render exactly these strings
- Product name: "MERIDIAN PAY"
- Date range: "JAN-JUN 2026"
- Account chip: "Acme Ltd"
- Navigation, top to bottom: "Overview" / "Payments" / "Payouts" / "Customers" / "Risk" / "Settings"
- KPI tile 1: "NET VOLUME" then "$4.82M" then "+12.4%"
- KPI tile 2: "ACTIVE ACCOUNTS" then "18,204" then "+3.1%"
- KPI tile 3: "AUTH RATE" then "97.6%" then "-0.4%"
- KPI tile 4: "SETTLEMENT TIME" then "1.9 days" then "-0.3 days"
- Line chart title: "Volume and refunds"; its legend entries: "Gross volume" and "Refunds"
- Line chart x-axis ticks, left to right: "JAN" "FEB" "MAR" "APR" "MAY" "JUN"
- Line chart y-axis: four labelled ticks ascending bottom to top: "0", "1M", "2M", "3M"
- Bar chart title: "Payouts by rail"; its legend entries: "ACH", "Card", "Wire"
- Table headers, in order: "TRANSACTION ID" "MERCHANT" "RAIL" "AMOUNT" "STATUS" "SETTLED"
- Table rows, in order:
  "TXN-8842" "Kestrel Supply" "ACH" "$12,400.00" "Settled" "04 Jun"
  "TXN-8843" "Northgate Ltd" "Card" "$8,150.50" "Settled" "05 Jun"
  "TXN-8844" "Albion Works" "Wire" "$21,900.00" "Pending" "06 Jun"
  "TXN-8845" "Vantage Foods" "ACH" "$5,320.75" "Settled" "06 Jun"
  "TXN-8846" "Ridgeway Co" "Card" "$2,900.25" "Failed" "07 Jun"
- Table footer: "Showing 1-5 of 312" at the left and "Subtotal $50,671.50" at the right

TYPOGRAPHY
One UI sans throughout, five sizes only: page-level product name, KPI value, panel title, table and axis text,
and small labels. Numerals are tabular. The AMOUNT column is right-aligned; all other columns are left-aligned.
KPI values are right-aligned within their tiles. All text is horizontal.

RENDERING
Flat interface rendering: no photographic lighting, no reflections, no glass, no bevels, no gradients. Ground
"#FBFAF8", body text "#1C1B19", one accent "#3D6B4F" used only for the active nav bar, the positive deltas and
the primary chart series; negative deltas in a muted "#B4442E". Hairline borders in "#E3DFD8". A 1 px grid of
faint horizontal rules in the table only.

CONSTRAINTS
Render only the strings listed above. Do not invent a metric, a merchant, a transaction, a menu item, a column,
a tooltip, a notification badge or a footnote. Do not use lorem ipsum, "TBD", "xx,xxx" or placeholder dashes.
Every chart must have both labelled axes and legend entries that match the series actually drawn. No two table
rows may share a transaction ID and no value may repeat verbatim in two rows of the same column. No browser
chrome, no OS status bar, no notch, no cursor, no selection highlight, no watermark. Do not round or reformat
any figure, and do not change a single digit.
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Ask for internal consistency, not just plausible numbers.** Each KPI's delta sign has to agree with the direction of its own sparkline; the five table amounts have to sum to the total printed in the footer. Both requirements are checkable in the finished frame, and both are what separate a mock someone can use from one that falls apart when a client reads it.
- **State the arithmetic explicitly.** Writing out that the five amounts sum to exactly $50,671.50 is what makes the footer figure correct rather than decorative. Give the model the answer, not the instruction to find one.
- **Ban the placeholder vocabulary by name.** Lorem ipsum, "TBD", "xx,xxx" and dashes standing in for data are what a mock reaches for when it runs out of concrete strings. Naming them is what stops it.

## Settings and result

`gpt-image-2.5-sunburst` · 4K requested · 16:9 · **3840 × 2160 px** · 38.4 s

Every string rendered correctly. `MERIDIAN PAY`, `JAN-JUN 2026` and the `Acme Ltd` chip in the top bar; all six navigation items with `Overview` correctly marked active by both a tinted row and a left accent bar; all four KPI tiles with their labels, values and deltas; both chart titles and all five legend entries; all six axis ticks on the x-axis and all four labelled ticks on the y-axis; all six table headers; all five table rows complete and character-perfect; and the footer reading `Showing 1-5 of 312` on the left and `Subtotal $50,671.50` on the right.

The consistency requirements held, which matters more than the typography. All four sparklines move in the direction their own delta sign claims — rising for net volume and active accounts, falling for auth rate and settlement time — so a reader checking the tiles finds nothing contradictory. The line chart's two drawn series match its two legend entries exactly, and the bar chart's three series appear in every column. The five table amounts are exactly $12,400.00, $8,150.50, $21,900.00, $5,320.75 and $2,900.25, which sum to $50,671.50 — the figure printed in the footer. No transaction ID repeats, and no value repeats within a column.

The rendering is a flat interface with no photographic lighting, one accent green on the active nav item and the positive deltas, and a muted red reserved for the negative ones.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
