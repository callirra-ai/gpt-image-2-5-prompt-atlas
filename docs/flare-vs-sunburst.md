# Flare vs Sunburst: a controlled comparison

GPT Image 2.5 ships as two tiers. OpenAI describes them by their priorities rather than
their output:

| Tier | Positioning |
|---|---|
| **Flare** | the speed-oriented tier — "high-volume everyday generation, creator content, and rapid prototyping" |
| **Sunburst** | the precision-oriented tier — "detailed creative work where editing accuracy matters more than generation speed" |

Both cost the same per token. Neither description tells you which one to pick for a given
image, and we could not find anyone who had measured the difference rather than repeated the
marketing copy. So we ran five prompts through both tiers, at the same settings, and looked.

## Method

Same prompt, same aspect ratio, same `quality: "xhigh"`, one variable: the tier. Five prompts
were chosen to fall on different sides of the claimed split — three photographic, two
interface/diagram:

| Case | Prompt | Why it is in the test |
|---|---|---|
| [16 Direct Flash Night Portrait](../showcase/16-direct-flash-night-portrait/) | 117 words | pure light — a hard single source with nowhere to hide |
| [17 Night Market Queue](../showcase/17-night-market-queue/) | 81 words | three mixed colour temperatures at once |
| [18 Golden Hour Backlight](../showcase/18-golden-hour-backlight/) | 72 words | flare and rim light, a second light test from a different angle |
| [19 Retro Racing Game Replay](../showcase/19-retro-racing-replay/) | 109 words | five exact HUD strings — the text-precision claim |
| [20 Isometric Dungeon Key Art](../showcase/20-isometric-dungeon-key-art/) | 131 words | dense structured layout — the geometry claim |

---

## Case 16 — Direct Flash Night Portrait

![Flare](../showcase/16-direct-flash-night-portrait/preview-flare.jpg)

![Sunburst](../showcase/16-direct-flash-night-portrait/preview-sunburst.jpg)

Both tiers get the hard light right: flat illumination, a shadow thrown straight onto the wall,
the background falling to black. **Flare holds the skin better** — pores, freckles and the oily
highlight across the forehead are individually visible, where Sunburst renders a marginally
smoother face. The wet pavement return is present in both.

**Flare wins, narrowly.** The tonal rendering matters more than the composition in a portrait
whose entire subject is one light source.

## Case 17 — Night Market Queue

![Flare](../showcase/17-night-market-queue/preview-flare.jpg)

![Sunburst](../showcase/17-night-market-queue/preview-sunburst.jpg)

A closer call. Flare resolves the steam and the crowd into separate layers and keeps the stall
readable behind them; Sunburst tightens the framing and gives slightly more definition to the
cooking equipment. Three colour temperatures — sodium bulbs, a cold spill, the warm griddle —
survive in both.

**Effectively a tie.** This prompt does not separate the tiers.

## Case 18 — Golden Hour Backlight

![Flare](../showcase/18-golden-hour-backlight/preview-flare.jpg)

![Sunburst](../showcase/18-golden-hour-backlight/preview-sunburst.jpg)

**The clearest separation in the set.** Flare puts a real flare streak across the frame and
turns the hair into a rim that reads as light rather than as a painted edge. Sunburst gives a
flatter, more even result — pleasant, but it stops looking like a lens and starts looking like
a gradient.

**Flare wins clearly.** Anything whose value depends on how light behaves in air is Flare's.

## Case 19 — Retro Racing Game Replay

![Flare](../showcase/19-retro-racing-replay/preview-flare.jpg)

![Sunburst](../showcase/19-retro-racing-replay/preview-sunburst.jpg)

**Both tiers placed all five strings correctly** — `3/8`, `LAP 2/5`, `0'47"12`, `0'45"88`,
`241 km/h`. No typos, no substitutions, on either tier.

**The layout is where they part.** Sunburst stacks every readout into one tight block at the top
right, in yellow-on-white with a dark outline, and gives the speed readout a segmented
instrument bar. Flare scatters the same five readings into all four corners in flatter white
type and puts the speed number on top of its own bar.

**Sunburst wins clearly.** For anything with an interface in it, this is the tier.

## Case 20 — Isometric Dungeon Key Art

![Flare](../showcase/20-isometric-dungeon-key-art/preview-flare.jpg)

![Sunburst](../showcase/20-isometric-dungeon-key-art/preview-sunburst.jpg)

Both produce a legible three-level cutaway at 30 degrees with the warm/cold light split and a
single lamp-carrying figure on the stair. Sunburst resolves the cut walls, roots and rubble
more distinctly.

**Sunburst wins, narrowly.** The margin is small — the least tier-sensitive card in the set.

---

## What we found

| Case | Winner | Margin |
|---|---|---|
| 16 Direct Flash Night Portrait | **Flare** | narrow |
| 17 Night Market Queue | tie | — |
| 18 Golden Hour Backlight | **Flare** | clear |
| 19 Retro Racing Game Replay | **Sunburst** | clear |
| 20 Isometric Dungeon Key Art | **Sunburst** | narrow |

The boundary is not photography-versus-design, and it is not the word count. It is **whether the
image's value lives in how light behaves or in how things are arranged**:

- **Flare** renders atmosphere. Highlights bloom, flare streaks, and a single hard source produces
  a believable falloff. It contributes atmosphere the prompt did not specify.
- **Sunburst** renders structure. Type sits on the baseline, interface elements align to a grid,
  and a layout does not drift. It contributes order the prompt did not specify.

They cost the same, so the practical rule is a one-line decision at the point of writing the
prompt:

> **If the picture is about light, use Flare. If the picture is about arrangement, use
> Sunburst.** When a prompt is genuinely both — a lit scene that also has to be precise — pick
> the axis you cannot fix afterwards: resolution and layout can be corrected downstream, light
> cannot.

## Reproducing this

Every render in this comparison is committed with its settings:

- Prompts: `showcase/<case>/prompt.txt`
- Per-render records: `showcase/<case>/generation-or-flare.json`, `generation-or-sunburst.json`
- Full-size files: `showcase/<case>/full-flare.jpg`, `full-sunburst.jpg`

Both tiers were requested through OpenRouter (`openai/gpt-image-2.5-flare` /
`openai/gpt-image-2.5-sunburst`) at `quality: "xhigh"`. Note that OpenRouter's GPT Image 2.5
endpoints do not expose a resolution parameter, so every frame here is **1536 × 1024** for a
3:2 aspect — a limitation of that route rather than of the model.

---

[← Back to the gallery](../README.md)
