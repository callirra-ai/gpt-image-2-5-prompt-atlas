# Lunar Courier — Character Sheet

![A character design sheet with four views of a courier, each zone showing the same character and equipment](preview.jpg)

A character design sheet in four zones — three-quarter front, side, back, and the pack laid out flat — for a lunar courier in a cream cape with a cobalt hard-shell pack and a single orange tool box. Use it for game and animation character bibles, art-direction pitches, and any sheet where the same design has to survive being turned around.

**This case is also a worked example of a real failure**, because the first render got the asymmetry wrong — and the cause was the prompt, not the model. See the result note below.

## Try the prompt

```text
A character design sheet for a lunar courier, drawn on a 3:2 landscape sheet of warm off-white design paper at a
slightly larger scale than a technical reference: four zones, each with a clear border of empty space, hand-drawn
production-art quality, flat cel shading with a single light source from the upper left.

THE CHARACTER — reproduce identically in every view
A courier of about thirty, wiry build, medium height, close-cropped dark hair, a narrow face with a strong
jawline and a thin scar through the left eyebrow. Wearing a cream short cape that stops at the hip with a
scuffed brass clasp at the throat, a slate-grey flight suit with a high collar and ribbed cuffs, worn carbon
boots scuffed at the toe, and fingerless gloves.

Equipment: a hard-shell backpack in cobalt blue with a visible seam, two side pockets and a rolled blanket
strapped on top, and — the asymmetric detail — a single orange tool box clipped to the character's RIGHT hip.
Nothing is worn on the left hip.

THE HIP SIDE — read this before drawing any view
The orange tool box is on the character's OWN RIGHT hip. A figure facing the viewer is mirrored, so the two
views must show it on opposite sides of the sheet:
- FRONT or three-quarter-front view: the box appears on the **LEFT** side of the sheet.
- BACK view: the box appears on the **RIGHT** side of the sheet.
- SIDE view: the character faces the **viewer's right**, so that the right hip is the near side and the box is
  visible in profile at the front of the hip.
Never draw the box on the same side of the sheet in the front view and the back view. Getting this wrong is the
single failure that ruins the sheet.

ZONE 1 — main three-quarter front view, upper LEFT of the sheet, the largest figure
Full body, standing, weight on the left leg, turned about thirty degrees, head facing the viewer, arms relaxed.
The orange tool box reads on the left side of the sheet. Both hands are empty and open.

ZONE 2 — side view, upper RIGHT of the sheet
Full body, facing the viewer's right, standing straight, arms at the sides. The backpack's profile is visible:
its depth, the two side pockets, the rolled blanket on top. The orange tool box is visible on the near hip.

ZONE 3 — back view, lower centre-left of the sheet, roughly a third smaller than Zone 1
Full body, seen from directly behind. The cape falls open at the back, the backpack covers the upper back with
its straps crossing at the chest, and the rolled blanket sits on top of it. The orange tool box appears on the
RIGHT side of the sheet.

ZONE 4 — equipment detail, lower right of the sheet, no figure
The backpack shown on its own, opened: the main compartment, the two side pockets, and the internal divider
laid out flat. Drawn at about half the size of the backpack in Zone 2 and consistent with it in every
proportion, seam position and colour. Nothing else is drawn in this zone.

SHEET PRESENTATION
Drawn figures and equipment only, on flat design paper. No grid lines, no measurement rulers, no dimension
arrows, no callouts, no leader lines. Line work is confident and slightly varied in weight; shadows are a single
flat tone per material, not rendered gradients. The paper has a faint tooth and a soft uneven edge where the
sheet meets the background.

CONSTRAINTS
No text anywhere: no labels, no names, no view captions, no colour swatches with codes, no watermark, no
signature. The character's face, hair, cape, suit, boots and both pieces of equipment must be identical across
Zones 1 to 3 — same proportions, same colours, same seam positions. The backpack in Zone 4 must match the
backpack as worn in Zones 1 to 3. Do not mirror the orange tool box between the front and back views. Do not add
a second character, a pose sheet, a turnaround strip, a colour palette strip, or a background environment.
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **State the mirroring rule explicitly, and state it correctly.** This is the sentence that makes or breaks a turnaround sheet: *an item on the character's right hip appears on the **left** of the frame in the front view and on the **right** of the frame in the back view.* Leave it out, or write it the wrong way round, and the sheet will show the same asymmetry on the same side in opposing views.
- **Draw the sheet before you trust it.** Check the one asymmetric detail by looking at where it falls in the front view and where it falls in the back view. Every other element can be off-model and still pass at a glance; the mirrored asymmetry is the error a reviewer catches immediately.
- **Change the profession by changing the equipment, not the colours.** A courier, a surveyor and a medic differ in what is on the body and where it clips. Recolouring the same pack and box gives you a palette variant, not a new character.

## Settings and result

`gpt-image-2.5-sunburst` · 4K requested · 3:2 · **3520 × 2336 px** · 43.4 s (second attempt)

**The first attempt failed, and the fault was in the prompt.** It declared the orange tool box on the character's *right* hip while also requiring it to appear on the *viewer's right* in the front view. That is physically impossible — a figure facing the viewer is mirrored, so a right-hip item falls on the **left** of the frame. Handed a contradiction, the model kept the box on the same side of the sheet in the front and back views: exactly the failure the prompt forbade.

The fix was to stop describing what the viewer sees in the front view and state the rule instead: the box is on the character's own right hip; therefore it appears on the **left** of the sheet in the front view and on the **right** in the back view. The re-render followed it: the box sits on the left of the largest figure and on the right of the back view, which is the check this sheet exists to pass. The side view also came out facing the viewer's right, so the near hip is the correct one and the box reads in profile.

Everything else held on both attempts — cream cape with the brass clasp, slate-grey flight suit with ribbed cuffs, scuffed boots, cobalt pack with the rolled blanket on top, four zones with clear separation, and no text anywhere on the sheet. Zone 4 shows the pack both closed and opened with the side pockets and the flat internal divider.

Three non-core deviations are worth flagging honestly rather than hiding: the face reads younger than thirty and a little more conventionally heroic than "wiry", the scar through the left eyebrow is not clearly visible, and the gloves are drawn as full gloves rather than fingerless. None of those break the sheet's purpose, so it was kept rather than re-rolled.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
