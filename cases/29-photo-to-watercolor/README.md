# Photo to Watercolor

| Photograph | Watercolour |
|---|---|
| ![A photograph of a woman standing in a walled garden in late afternoon](reference-1.jpg) | ![The same scene repainted as a loose watercolour](preview.jpg) |

Repaint a photograph as an original watercolour at the same composition and framing, keeping the person recognisable and the light direction intact. Use it for portrait commissions, editorial illustration, wedding and family work, book covers, and the very common request to "turn this photo into a painting" without losing the likeness.

**This case documents a two-attempt process.** The first repaint changed the person; the note at the bottom says exactly what drifted and what fixed it.

## Try the prompt

```text
Image 1: the photograph — the sole authority for the composition, the pose, the framing, the direction of the
light and the identity of the person. It supplies no paint, no brushwork and no paper.

TASK
Repaint Image 1 as an original watercolour on rough cold-pressed paper, at the same composition and the same
framing, so that it reads as a painted study made from the photograph rather than a photograph with a filter
over it.

THE PERSON — preserve her exactly as she appears in Image 1
- Her hair is worn LOOSE and down, falling just past her jaw with a slight wave, with several strands lying
  across her cheek and one behind the ear. Her hair is NOT tied up: do not add a bun, a twist, a knot, a
  ponytail or a hair clip, and do not lift it off her neck.
- Her clothing is exactly as in the photograph: a pale sage linen shirt with the collar open, sleeves rolled to
  the elbow, tucked into DARK charcoal trousers. The trousers are dark. Do not lighten them, do not make them
  cream, beige or stone, and do not change them to a skirt.
- Both arms hang relaxed at her sides and BOTH HANDS ARE EMPTY AND VISIBLE, held slightly away from the body.
  Do not put a hand in a pocket, do not cross her arms, and do not hide either hand.
- The only bag in the picture is the thin dark leather STRAP crossing her right shoulder, visible where it
  passes over the shirt. There is no bag body visible, no tote bag, no canvas bag and no second strap.
- Her face: the same structure, the same narrow jaw, the same straight nose and eyebrow shape, and the same
  quiet expression with the mouth closed. Her gaze is directed off to the left of the frame.

PRESERVE — the setting and the light
- The wall runs from the near left into the distance at the same angle, and it is RED-BROWN BRICK with visible
  courses and mortar lines, with moss at its base. It is brick, not stone, not rough rubble and not concrete.
- The planting along the wall's base, the gravel path receding behind her, and the tops of the trees above the
  wall line in the same place.
- The sun comes from behind and to her left exactly as in Image 1: the rim of her shoulder, the edge of her hair
  and the fold of her sleeve are the brightest edges, and the long shadows fall on the gravel toward the right.
- The gravel is neutral grey and the brick is warm red-brown.

CHANGE — the medium, completely
- Paint, not pixels. Loose wet-in-wet washes laid in broad passages, pigment blooming where two washes meet,
  granulation settling visibly at those boundaries, and the paper's tooth showing through every wash.
- Several edges deliberately lost: the far end of the wall and the distant treetops dissolve into the paper with
  no line at all, and the gravel path fades out rather than being drawn.
- Whites are unpainted paper. There is no white body paint anywhere, and the brightest values come from areas
  where nothing was applied.
- A few dry-brush skips across the grain, and one or two places where the paper was left to dry before the next
  wash, so the boundary is crisp and irregular rather than soft.
- Palette limited to five pigments: warm ochre, burnt sienna, cool grey-blue, soft sage for the shirt, and one
  deep indigo for the darkest notes in her hair and the wall shadow.
- Figures are suggested, not detailed: her face is a small number of carefully placed shapes with the features
  read from value rather than from line, and her hands are simple masses with no drawn fingers.

DO NOT
- Do not restyle her hair, her clothing or her pose in any way. Do not add a bag, a hat, a scarf or sunglasses.
- Do not make it photographic: no sharp photographic detail, no photographic grain, no lens blur, no depth of
  field, no noise and no digital gradient.
- Do not smooth her face into a generic pretty face, and do not change her apparent age.
- Do not change the direction of her gaze or the direction of the light.
- Do not add people, animals, a gate, a doorway, a bench, a bicycle or flowers in her hands.
- Do not sign it, date it, add a stamp or a watermark, and do not paint a white border around the picture.
```

The photograph is generated for this case, so the whole recipe is reproducible — its prompt is in [`reference-prompt.txt`](reference-prompt.txt).

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Name what stays, item by item, and write it as a prohibition.** "LOOSE and down, falling just past her jaw … NOT tied up: do not add a bun" is what fixed this case. The first attempt said "the same hairline and the same loose strands" and got a bun.
- **Spend most of the prompt on the person and the light, only a paragraph on the medium.** The medium conversion is the easy part for a model; keeping the subject recognisable and the light direction correct is the part that fails.
- **Say "paint, not pixels" and then give the specific behaviours.** Wet-in-wet blooming, granulation at the wash boundaries, lost edges, dry-brush skips, unpainted paper for whites. A style name alone gets you a photograph with a watercolour filter over it.

## Settings and result

`gpt-image-2.5-sunburst` · 2K requested · 2:3 · **1664 × 2512 px** · 40.6 s (second attempt) · reference uploaded and passed in order

**The first attempt was rejected, and the fault was in the prompt.** It asked to preserve "her hairline and the same loose strands across the cheek" — and got her hair pinned up in a bun. The trousers came back pale cream instead of charcoal, one hand went into a pocket, a large canvas tote appeared on her arm, and the brick wall turned into rough stone. The medium conversion itself had worked; the person had not survived it.

The fix was to stop describing and start forbidding, with the specific wrong outcome named: *her hair is worn loose and down … it is NOT tied up: do not add a bun, a twist, a knot, a ponytail or a hair clip*; *the trousers are dark — do not lighten them, do not make them cream, beige or stone*; *both hands are empty and visible — do not put a hand in a pocket*; *the only bag is the thin dark leather strap — there is no bag body visible*; *it is brick, not stone, not rough rubble, not concrete*.

The second render holds all of it. Her hair falls loose past the jaw with strands across the cheek, the trousers are dark charcoal, both hands hang empty and visible at her sides, only the thin leather strap crosses her shoulder, and the wall is red-brown brick with visible courses, mortar and moss at its base. The composition, framing and light direction are unchanged — the sun still comes from behind and to her left, rimming her shoulder, hair and sleeve, with the long shadows falling on the gravel toward the right.

The medium is a genuine watercolour rather than a filter: broad wet-in-wet passages with pigment blooming at the washes' edges, granulation settled along those boundaries, the paper's tooth showing through, several edges deliberately lost into bare paper, and whites that are simply where nothing was painted.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
