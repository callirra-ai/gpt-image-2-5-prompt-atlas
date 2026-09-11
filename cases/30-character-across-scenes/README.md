# Character Across Scenes

| Image 1 — person | Image 2 — pose | Image 3 — place and light | Result |
|---|---|---|---|
| ![A neutral identity portrait of a field botanist](reference-1.jpg) | ![A seated pose reference](reference-2.jpg) | ![A misty pine clearing at dawn](reference-3.jpg) | ![The botanist seated on the bridge abutment in the clearing](preview.jpg) |

Three references, three separate jobs: one says **who**, one says **how**, one says **where and in what light** — and the result has to satisfy all three at once. Use it for story illustration, game and film key art, brand campaigns with a recurring character, and any composite where a described person has to appear somewhere specific without losing their face.

**This is the flagship reference-discipline case in the atlas.** Every role is written down, and so is the rule for what happens when two of them disagree.

## Try the prompt

```text
Image 1: the person — the sole authority for who she is: her face, her age, her hair and the braid, her glasses,
her freckles, the scar on her jaw, and the clothing she wears. It supplies no pose, no place and no light.
Image 2: the pose — the sole authority for how she is arranged: the seated posture, the turn of the body, the
position of the limbs, the position of the head, and the framing of the shot. It supplies no identity and no
environment.
Image 3: the place and the light — the sole authority for the space, the camera position within it, the scale of
everything, the atmosphere and the direction and quality of every light. It supplies no person.

TASK
Paint the botanist from Image 1 seated in the pose from Image 2 on the low stone abutment of the footbridge in
Image 3, lit by that clearing's dawn light.

CONFLICT POLICY — read this before composing
- Image 1 wins on identity and on the appearance of her clothing, hair, glasses and the braid. Her freckles,
  the scar and the braid's side must not change.
- Image 2 wins on the pose and on where the frame is cut, so both feet stay inside the picture.
- Image 3 wins on everything about the world: the depth of the fog, the wetness of the ground, the direction of
  the light and the colour of the atmosphere.
- Where Image 1 and Image 3 disagree about colour, Image 3 wins on the light falling on her and Image 1 wins on
  the hue of the garment itself: a sage shirt stays sage, but its shading is derived from the clearing.
- Where Image 2 and Image 3 disagree about scale, Image 3 wins, so the bridge and the trunks keep their size
  and the figure is scaled to them.

PRESERVE EXACTLY
- Her face: the same structure, the same freckles across the nose and both cheekbones, the same round wire
  glasses, and the braid over the same shoulder ending at the same length.
- Her clothing: the same dark green canvas jacket with its corduroy collar, worn open at the throat over the
  same grey shirt, and the same dark trousers.
- The pose: seated, body turned a quarter to the right, leaning forward with both forearms on the thighs, left
  foot flat on the ground, right foot slightly back, head turned to look off to the right.
- The place: the clearing's pine trunks receding into fog, the needle floor, the ferns, the shallow stream, the
  timber footbridge on its two low stone abutments, and the fog thickest at about eight metres' depth.
- The light: one low sun outside the frame to the upper left, filtered through fog so it is diffuse and
  volumetric rather than hard, with everything near the light band warm and everything nearer and further away
  cool blue-grey.

MATCH NATURALLY
- She sits ON the stone abutment: her weight compresses the moss there, and her shadow falls on the stone
  beneath her, agreeing with the light coming from the upper left.
- Her shadow joins the long trunk shadows already running toward the lower right; she casts no shadow of her own
  in a different direction.
- Fog behaves with depth: she sits behind the nearest fog and in front of the thickest band, so her silhouette
  is slightly softened at its edges and the ground between her and the camera is a little lighter than the
  ground beyond her.
- Her jacket's damp-weather behaviour matches the clearing: canvas takes on a faint sheen where the fog settles
  and a slight darkening at the shoulders.
- Colour temperature: her rim light is warm pale gold because the sun is behind and above her left shoulder;
  everything facing the camera is lit only by the cool ambient fog, so her face is cool and her edges are warm.
- Grain, focus and contrast identical to the surrounding scene.

DO NOT
- Do not change her identity, her age, her build, or the side the braid falls on.
- Do not change the pose, add a hand on a rail, straighten her spine, or stand her up.
- Do not change the bridge, the stream, the trunks, the fog's depth, the camera height or the direction of the
  light.
- Do not add a second person, a dog, a backpack, a tripod, a notebook, a campfire, a tent or litter.
- Do not introduce hard sun shafts or god rays; the light is diffuse in fog.
- Do not add colour accents that are not in Image 3, and do not warm the whole frame.
- No text, no signage, no watermark.
```

All three references were generated for this case, so the whole recipe is reproducible — their prompts are in [`reference-prompt-1.txt`](reference-prompt-1.txt), [`reference-prompt-2.txt`](reference-prompt-2.txt) and [`reference-prompt-3.txt`](reference-prompt-3.txt).

> **Reference order matters.** Attach them as Image 1, Image 2 and Image 3 in that order. Same three files in a different order is a different request.

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Give every reference one job and say what it must not supply.** *Image 2 supplies no identity and no environment.* That clause is what stops the pose reference's own background bleeding into the picture, and it is the single most useful line in the prompt.
- **Write the conflict policy as numbered rules.** Who wins on colour, who wins on scale, who wins on the light falling on her versus the hue of the garment. Without it the model averages the references and the face drifts toward the pose reference's own model.
- **Make the subject touch the world.** She sits *on* the abutment, her weight compresses the moss, her shadow falls on the stone beneath her and joins the trunk shadows already there. Contact is what moves a figure from pasted to present.

## Settings and result

`gpt-image-2.5-sunburst` · 4K requested · 2:3 · **2336 × 3520 px** · 40.9 s · three references uploaded and passed in order

All three roles held simultaneously, which is what this case exists to demonstrate.

**From Image 1:** the same face and build, the dark auburn hair with the braid falling on the same shoulder to the same length, the round wire-rimmed glasses, the freckles across the nose and cheekbones, and the dark green canvas jacket with its corduroy collar, worn open over the grey shirt with the same dark trousers.

**From Image 2:** the seated pose on the low stone abutment, body turned a quarter to the right, leaning forward with both forearms resting on the thighs, the left foot flat on the ground and the right slightly back, head turned to look off to the right, with both feet inside the frame.

**From Image 3:** the pine clearing receding into fog, the needle floor, the ferns, the shallow stream, the timber footbridge on its two low stone abutments, the fog thickest at about eight metres' depth, and the light — one low sun outside the frame to the upper left, filtered through fog, so the rim on her shoulder and hair is warm pale gold while everything facing the camera is cool ambient, with the long trunk shadows running toward the lower right.

The contact requirement came through as well: she sits on the stone with the moss compressed under her weight and her shadow falling on the abutment beneath her, joining the trunk shadows already crossing the ground rather than pointing somewhere of its own. One small drift: the hands meet in front of her rather than being tucked behind the opposite knee as the pose reference specifies, which is worth knowing if hand placement matters to your use.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
