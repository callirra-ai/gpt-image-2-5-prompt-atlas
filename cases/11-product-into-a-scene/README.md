# Product Into a Scene

| Image 1 — product | Image 2 — scene | Result |
|---|---|---|
| ![A cream stoneware pour-over dripper on a plain background](reference-1.jpg) | ![An oak kitchen counter with morning light from the left](reference-2.jpg) | ![The dripper placed on the counter, lit by the window](preview.jpg) |

Put your product into a real scene using two references — one for the product, one for the place — with each reference given exactly one job. Use it for e-commerce lifestyle images, campaigns and catalogue work where the product has to look photographed on location rather than cut out and pasted.

This is the reference-discipline case: **Image 1 is the only source of the object, Image 2 is the only source of the world, and neither is allowed to do the other's job.**

## Try the prompt

```text
Image 1: the product — the sole authority for the dripper's form, its proportions, its cream glaze, the throwing
line, the interior ribs, the drain hole, the unglazed foot and the shape of the side handle. It supplies no
setting, no camera and no lighting.
Image 2: the scene — the sole authority for the space, the counter, the camera position, the scale of everything
in frame and the direction and quality of every light. It supplies no product.

TASK
Place the dripper from Image 1 onto the clear strip of counter along the front edge of Image 2, standing upright
on its foot at the left third of the frame, and follow the scene's own light exactly.

PRESERVE EXACTLY
- The dripper's geometry: cone angle, rim diameter, base ring, handle size and its angle, the wall thickness at
  the rim, and the interior ribs and drain hole.
- The dripper's material: cream glaze with the same gloss level, the same visible throwing line, the same
  slightly uneven rim, the same unglazed clay foot.
- The scene: the oak worktop with its grain, knife marks and water ring, the tiled splashback, the wall above
  it, the enamel kettle, the folded linen cloth, the bowl of beans and their positions.
- The camera: identical position, height, angle and framing. The result must align with Image 2 edge to edge.
- The empty strip of counter along the front edge stays otherwise empty.

MATCH NATURALLY
- Light direction: the window is off-frame to the left, so the dripper is lit from the left. Its lit side is on
  the left, its shadow falls to the right, and its right side falls into the same gentle gradient as the
  splashback behind it.
- Colour temperature: warm in the highlight, cool in the shadow, matching the rest of the scene. Do not add a
  warm or cool cast of its own.
- Contact shadow: one soft-edged shadow beneath the base, short and to the right of the object, denser where the
  foot ring meets the counter and fading outward.
- Reflection: a faint, low-contrast reflection of the base in the oiled oak immediately beneath it, the same
  intensity as the reflection the kettle already casts.
- Scale: the dripper is roughly the height of the enamel kettle's body and stands on the same plane, its base
  resting on the counter surface at the same depth as the kettle's base. It must not float or sink.
- Grain and sharpness: identical to the rest of the frame at the same depth.

DO NOT
- Do not redesign, restyle, recolour or reshape the dripper, and do not change its glaze or its handle.
- Do not change the counter, the splashback, the existing three objects, the camera, the crop or the light
  direction.
- Do not add coffee, a filter, a mug, beans, a spoon, steam, a hand or a second product.
- Do not paste the object flat: no outline, no cut-out edge, no drop shadow of even density, no missing contact
  shadow, no flat colour fill.
- Do not apply a shadow that disagrees with the light coming from the left.
- No text, no logo, no watermark.
```

Both references were generated for this case, so the whole recipe is reproducible — their prompts are in [`reference-prompt-1.txt`](reference-prompt-1.txt) and [`reference-prompt-2.txt`](reference-prompt-2.txt).

> **Reference order matters.** Attach them as Image 1 and Image 2 in that order. Same two files, swapped, is a different request.

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Give each reference exactly one job, and say what it must not supply.** Image 1 owns the object; Image 2 owns the space, the camera and every light. The moment two references can both decide the light, the model averages them and the product stops matching its own reference.
- **Match the light by naming its behaviour, not its mood.** "Lit from the left, shadow to the right, cool in the shadow, warm in the highlight, reflection as strong as the one the kettle already casts" is checkable. "Cinematic lighting" is not.
- **Ask for a contact shadow and a reflection, always.** Their absence is what makes a composite look pasted. Their presence, at the right intensity, is most of what makes it look shot.

## Settings and result

`gpt-image-2.5-sunburst` · 4K requested · 3:2 · **3520 × 2336 px** · 37.5 s · references uploaded and passed in order

The dripper from Image 1 is on the counter from Image 2, upright on its own foot at the left third, at roughly the height of the enamel kettle's body and resting on the same plane. The scene is otherwise untouched: the oak worktop with its grain and knife marks, the tiled splashback, the kettle, the folded linen cloth and the bowl of beans are all where they were.

The lighting is the part that decides whether a composite works, and it followed the reference rather than the prompt's hopes: the dripper is lit from the left, its shadow falls to the right and sits under the base as a soft contact shadow, and a faint reflection appears in the oiled oak beneath it at the same strength as the kettle's. The cream glaze keeps its warm highlight and cool shadow, so the object belongs to the room instead of sitting on top of it.

One drift is worth naming: the dripper's base came out simpler than the reference — the distinct wide foot ring reads as a smaller base and the interior shows more ribs than the three the reference has. The object still reads unmistakably as the same hand-thrown piece, so the case was kept, but if a product's base geometry is commercially sensitive, expect to state it twice or to finish by hand.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
