# Sixteen-Pose Contact Sheet

![A 4×4 contact sheet of the same character in sixteen different standing poses](preview.jpg)

Sixteen panels of the same character in sixteen different standing poses, shot on one camera that never moves, so the ground line and the head height are identical in every panel. Use it for character bibles, animation reference, casting boards, rigging reference and any sheet where consistency across many panels is the whole point.

## Try the prompt

```text
A character pose contact sheet, 1:1 square, sixteen panels in a 4 by 4 grid with even gutters and a thin dark
outer border. Each panel shows the same person in a different standing pose, photographed on a plain mid-grey
seamless with flat even lighting. This is a reference sheet, not a beauty photograph.

THE CAMERA — identical in all sixteen panels
One camera, one position, never varied: eye level at 60% of the figure's height, straight on, 85 mm equivalent,
no wide-angle distortion, no tilt, no zoom change, no perspective change between panels. Because the camera and
the distance never move, the ground line falls at exactly the same height in all sixteen panels and the top of
the head falls at exactly the same height in all sixteen panels. The figure is centred horizontally in every
panel with even margins left and right, and the feet are inside the panel in all sixteen.

THE CHARACTER — identical in all sixteen panels
A woman of about thirty, athletic build, medium height. Short dark hair cut to the jaw with a blunt fringe, a
thin scar on her LEFT forearm about four centimetres long, and a small mole on her RIGHT cheekbone. She wears
a plain charcoal cotton t-shirt with a crew neck, olive cargo trousers with a single pocket flap on the LEFT
thigh only, and tan canvas boots laced to the ankle. Her clothing, hair, scar and mole must be identical in
every panel, and the pocket flap must stay on the left thigh in all sixteen — it must never appear on the right.

THE SIXTEEN POSES, reading left to right then top to bottom
1. Neutral stance, feet shoulder-width apart, arms hanging at her sides.
2. Weight on the left leg, right knee slightly bent and relaxed, arms at her sides.
3. Feet together, hands clasped in front of her at waist height.
4. Feet apart, arms folded across her chest.
5. Left hand on her hip, right arm hanging down.
6. Right hand on her hip, left arm hanging down.
7. Both hands on her hips, elbows out, feet apart.
8. Left arm raised forward, pointing at chest height, right arm down.
9. Right arm raised straight up above her head, left arm down.
10. Both arms raised out to the sides at shoulder height, palms down.
11. Leaning forward from the hips, both hands resting on her thighs.
12. Standing turned a quarter away, looking back over her right shoulder.
13. Half crouch, knees bent, weight low, both arms held forward.
14. Standing up on the balls of both feet, heels off the ground, arms swung back.
15. Right foot forward a full stride, torso twisted to the left, arms loose.
16. Standing straight, both hands clasped behind her back.

PANEL NUMBERS
A small numeral in the bottom left corner of each panel, reading 1 to 16 in order, all the same size and in the
same position within their panels. These numerals are the only text on the sheet.

LIGHTING
One large soft source directly in front of the figure and slightly above, plus a soft fill from both sides, so
the lighting is even and flat and identical in all sixteen panels. One short soft shadow directly beneath each
figure, the same shape and length everywhere. No dramatic lighting, no coloured light, no rim light, no change
of exposure between panels.

CONSTRAINTS
All sixteen panels are present and all sixteen poses are different. No sitting, kneeling, lying, jumping or
airborne pose: both feet are on the ground in every panel. Do not hide the feet, do not crop the head, and do
not let the figure leave the panel. Do not mirror the character's asymmetric details between panels — the scar
stays on the left forearm and the mole stays on the right cheekbone in all sixteen. Do not add props, weapons,
bags, hats, furniture or a background other than the plain seamless. No text anywhere except the sixteen panel
numerals, and no number larger than 16.
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Spend the prompt on the camera, not on the poses.** "One camera, one position, never varied: eye level at 60% of height, straight on, no zoom change between panels" is what makes sixteen panels comparable. The poses are the easy part — the identical framing is the hard part, and without it the sheet is sixteen photographs instead of one reference.
- **Give every pose a number and check them off.** Sixteen numbered poses listed in reading order means you can verify the sheet in under a minute. A prose description of "various standing poses" gets you six poses and a lot of empty panels.
- **Keep the feet on the ground.** Standing, weight-bearing, both feet planted, no sitting or jumping. Ground contact is what makes a pose sheet usable for rigging, and it removes the whole class of floating-body failures.

## Settings and result

`gpt-image-2.5-sunburst` · 4K requested · 1:1 · **2880 × 2880 px** · 39.9 s

All sixteen panels are present in the correct 4×4 grid and **all sixteen poses are distinct and in the stated order** — neutral, weight-shifted, hands clasped, arms folded, left hand on hip, right hand on hip, both hands on hips, left arm pointing, right arm overhead, both arms out to the sides, leaning forward with hands on thighs, turned away looking over the shoulder, half crouch, up on the balls of the feet, striding with a torso twist, and standing with hands behind the back. The panel numerals read 1 to 16 with none missing and none repeated.

The camera requirement holds, which is what the case is built on: the ground line falls at the same height in every panel and the top of the head at the same height in every panel, so the sixteen figures are directly comparable rather than sixteen separate photographs. The character stays consistent throughout — the blunt dark bob, the charcoal crew-neck t-shirt, the olive cargo trousers and the tan canvas boots are the same in every panel.

One honest shortfall: the asymmetric detail used as the mirroring test does not survive at this scale. The trousers read as standard cargo trousers with pockets visible on both sides rather than the single left-thigh flap specified, and the forearm scar is not readable in the panels where the arms are visible. The sixteen-pose consistency, which is the case's actual purpose, is intact — but if you need a mirroring check on a sheet like this, put the asymmetry somewhere large and dark, not on a trouser leg.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
