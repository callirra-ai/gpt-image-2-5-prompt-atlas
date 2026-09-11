# Exploded Ramen Bowl

![A ramen bowl with seven components suspended above it in assembly order, each with a thin leader line to its label](preview.jpg)

An exploded assembly diagram of a ramen bowl: the finished bowl at the bottom, its seven components floating above it in the order they are assembled, each named by a single thin leader. Use it for menus, food-brand campaigns, packaging back panels and any product where the point is *what is in it*.

## Try the prompt

```text
A commercial food photograph of an exploded ramen bowl, drawn on a 4:3 canvas as a vertical assembly diagram
in three dimensions: the finished bowl at the bottom, and its components suspended above it in the order they
are assembled, each labelled.

COMPOSITION
Dark slate ground filling the frame, one value, with a soft pool of light in the centre. The ceramic bowl sits
in the lower third, centred, seen from a slightly raised three-quarter angle so its interior is visible. Directly
above the bowl, seven components float in a vertical stack with generous even gaps, largest at the bottom,
smallest at the top. Each component has one thin straight leader line running horizontally out to a label at
the left or right margin; no leader crosses another, no leader crosses a component, and every leader ends exactly
on the component it names.

THE COMPONENTS, bottom to top
1. Amber broth held as a perfect disc of liquid suspended in mid-air, with a defined meniscus and a bright
   highlight along its edge; faint steam rising from this disc only.
2. A coil of fresh noodles, lifted and separated so individual strands are visible, glossy and pale gold.
3. Three slices of braised pork belly, edge-seared, with visible fat-to-meat layering and a caramelised rim.
4. Two halves of a marinated soft-boiled egg, yolks jammy and slightly translucent, cut faces toward camera.
5. A sheet of toasted nori standing almost upright, matte black-green with visible fibre structure.
6. A small fan of sliced scallions, fresh green and white rings, crisp edges.
7. A tight cluster of chili oil droplets suspended together, each catching a small bright specular point.

TEXT — render exactly these seven strings, one per label, each appearing once
"BROTH" / "NOODLES" / "CHASHU" / "SOFT EGG" / "NORI" / "SCALLION" / "CHILI OIL"
Typography: one neutral uppercase sans, one size only, set horizontally, left-aligned on the left margin for
components 1, 3, 5, 7 and right-aligned on the right margin for components 2, 4, 6, so the leaders stay short.
No other text anywhere in the frame.

LIGHT AND MATERIAL
One large soft key from the upper left, one weak fill from the right, and one narrow back light that makes the
broth glow from within and catches the rim of the egg yolks. Ceramic: matte glaze with fine crazing and a soft
rim highlight. Liquid: glossy, opaque amber with a viscous meniscus. Noodles: wet and reflective without looking
oiled plastic. Pork: crisp caramelised edge, fibrous interior. Egg: dense jammy yolk with a matte albumen.
Steam rises only from the broth disc, thin and directional, never covering a component or a label.

CONSTRAINTS
Exactly seven components and exactly seven labels, one each, in the order given. Components must not overlap,
touch, or drift off the vertical axis. Do not add chopsticks, a spoon, a napkin, a second bowl, scattered
ingredients, flying droplets, herbs or decorative garnishes. Do not add brackets, arrows, dashed boxes,
measurement lines or dimension marks — the only graphics in the frame are the seven thin leaders. Do not
restyle the labels, do not add units or prices. No watermark, no logo, no border.
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **The count is the design.** Seven layers, seven labels, one each. If you add a component you must add its leader and re-space the stack; if you drop one, close the gap. An exploded diagram with an unlabelled layer stops being a diagram.
- **Alternate the leaders left and right.** That is what keeps them short and stops them crossing. All-left leaders on a stack this tall will tangle.
- **Swap the cuisine and rebuild the materials with it.** Ramen has liquid, gluten strands, fatty meat and a jelly yolk. A biryani, a burger or a sundae have completely different behaviours under light, and the material paragraph has to be rewritten rather than the nouns substituted.

## Settings and result

`gpt-image-2.5-sunburst` · 4K requested · 4:3 · **3312 × 2480 px** · 65.6 s

All seven components appeared in the correct assembly order and **all seven labels rendered correctly, once each** — `BROTH`, `NOODLES`, `CHASHU`, `SOFT EGG`, `NORI`, `SCALLION`, `CHILI OIL` — with the leaders alternating left and right and none crossing. For a frame with seven separate strings of English text that is the result that matters, and it is the reason this case is rendered at 4K.

The broth disc is the other thing worth noting: it holds a defined meniscus and a highlight along its edge, and it is the only component emitting steam. That single decision is what stops the stack from reading as seven flat cut-outs pinned to a wall. One honest caveat: the leaders for `SCALLION` and `SOFT EGG` run past the nori sheet at some distance, and at thumbnail size the middle of the stack reads a touch busy. Splitting the stack into two columns would fix it if you need a smaller rendering.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
